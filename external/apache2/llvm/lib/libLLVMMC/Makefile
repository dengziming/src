#	$NetBSD: Makefile,v 1.1 2019/11/11 22:45:08 joerg Exp $

LIB=	LLVMMC

.include <bsd.init.mk>

.PATH: ${LLVM_SRCDIR}/lib/MC

SRCS+=	ConstantPools.cpp \
	ELFObjectWriter.cpp \
	MachObjectWriter.cpp \
	MCAsmBackend.cpp \
	MCAsmInfoCOFF.cpp \
	MCAsmInfo.cpp \
	MCAsmInfoDarwin.cpp \
	MCAsmInfoELF.cpp \
	MCAsmInfoWasm.cpp \
	MCAsmInfoXCOFF.cpp \
	MCAsmMacro.cpp \
	MCAsmStreamer.cpp \
	MCAssembler.cpp \
	MCCodeEmitter.cpp \
	MCCodePadder.cpp \
	MCCodeView.cpp \
	MCContext.cpp \
	MCDwarf.cpp \
	MCELFObjectTargetWriter.cpp \
	MCELFStreamer.cpp \
	MCExpr.cpp \
	MCFragment.cpp \
	MCInst.cpp \
	MCInstPrinter.cpp \
	MCInstrAnalysis.cpp \
	MCInstrDesc.cpp \
	MCLabel.cpp \
	MCLinkerOptimizationHint.cpp \
	MCMachObjectTargetWriter.cpp \
	MCMachOStreamer.cpp \
	MCNullStreamer.cpp \
	MCObjectFileInfo.cpp \
	MCObjectStreamer.cpp \
	MCObjectWriter.cpp \
	MCRegisterInfo.cpp \
	MCSchedule.cpp \
	MCSectionCOFF.cpp \
	MCSection.cpp \
	MCSectionELF.cpp \
	MCSectionMachO.cpp \
	MCSectionWasm.cpp \
	MCSectionXCOFF.cpp \
	MCStreamer.cpp \
	MCSubtargetInfo.cpp \
	MCSymbol.cpp \
	MCSymbolELF.cpp \
	MCTargetOptions.cpp \
	MCValue.cpp \
	MCWasmObjectTargetWriter.cpp \
	MCWasmStreamer.cpp \
	MCWin64EH.cpp \
	MCWinCOFFStreamer.cpp \
	MCWinEH.cpp \
	MCXCOFFObjectTargetWriter.cpp \
	MCXCOFFStreamer.cpp \
	StringTableBuilder.cpp \
	SubtargetFeature.cpp \
	WasmObjectWriter.cpp \
	WinCOFFObjectWriter.cpp \
	XCOFFObjectWriter.cpp

.if defined(HOSTLIB)
.include <bsd.hostlib.mk>
.else
.include <bsd.lib.mk>
.endif
