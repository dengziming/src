#	$OpenBSD: Makefile,v 1.5 2015/10/21 06:37:25 doug Exp $

.include <bsd.own.mk>

# The larger ones will take many days, so if you're going to regen them run
# it in a tmux session or something.  The checkpoints should make it safe
# to stop and restart.
DHSIZE=2048 3072 4096 6144 7680 8192

.for bits in ${DHSIZE}
MODULI_PARTS+=moduli.${bits}
WORK_MODULI_PARTS+=${.OBJDIR}/moduli.${bits}.sieved.gz
.endfor



all:	${MODULI_PARTS}

update-moduli:	${MODULI_PARTS}
	( \
		echo -n '#    $$Open'; echo 'BSD$$'; \
		echo '# Time Type Tests Tries Size Generator Modulus'; \
		cat ${MODULI_PARTS} \
	) > ${BSDSRCDIR}/etc/moduli

clean:
	rm -f ${WORK_MODULI_PARTS}

.for bits in ${DHSIZE}
moduli.${bits}:
	sh ${.CURDIR}/moduli-gen.sh ${.CURDIR} ${.CURDIR}/work ${bits}
.endfor
