# Get directory of this makefile
MAKEFILE_DIR := $(dir $(lastword $(MAKEFILE_LIST)))

# Specify the default makedefs file, which can be overridden at the command line
MAKEDEFS = $(MAKEFILE_DIR)makedefs
include $(MAKEDEFS)

# Always builds phony rules
.PHONY: all clean

ifndef ADD_PARAM
ADD_PARAM=
endif

# Builds driverlib.lib
all :
		@ rm -f $(MAKEFILE_DIR)driverlib.lib
		@ rm -f $(MAKEFILE_DIR)*.o
		@ echo ADD_PARAM = \"$(ADD_PARAM)\"
		$(COMPILER_TOOL) --version
		@ echo IAR: Compile adi.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/adi.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)adi.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)adi.o $(MAKEFILE_DIR)adi.o
		@ echo IAR: Compile aes.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/aes.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)aes.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)aes.o $(MAKEFILE_DIR)aes.o
		@ echo IAR: Compile aon_batmon.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/aon_batmon.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)aon_batmon.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)aon_batmon.o $(MAKEFILE_DIR)aon_batmon.o
		@ echo IAR: Compile aon_event.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/aon_event.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)aon_event.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)aon_event.o $(MAKEFILE_DIR)aon_event.o
		@ echo IAR: Compile aon_ioc.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/aon_ioc.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)aon_ioc.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)aon_ioc.o $(MAKEFILE_DIR)aon_ioc.o
		@ echo IAR: Compile aon_pmctl.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/aon_pmctl.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)aon_pmctl.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)aon_pmctl.o $(MAKEFILE_DIR)aon_pmctl.o
		@ echo IAR: Compile aon_rtc.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/aon_rtc.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)aon_rtc.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)aon_rtc.o $(MAKEFILE_DIR)aon_rtc.o
		@ echo IAR: Compile aux_adc.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/aux_adc.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)aux_adc.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)aux_adc.o $(MAKEFILE_DIR)aux_adc.o
		@ echo IAR: Compile aux_dac.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/aux_dac.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)aux_dac.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)aux_dac.o $(MAKEFILE_DIR)aux_dac.o
		@ echo IAR: Compile aux_smph.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/aux_smph.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)aux_smph.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)aux_smph.o $(MAKEFILE_DIR)aux_smph.o
		@ echo IAR: Compile aux_sysif.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/aux_sysif.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)aux_sysif.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)aux_sysif.o $(MAKEFILE_DIR)aux_sysif.o
		@ echo IAR: Compile aux_tdc.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/aux_tdc.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)aux_tdc.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)aux_tdc.o $(MAKEFILE_DIR)aux_tdc.o
		@ echo IAR: Compile ccfgread.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/ccfgread.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)ccfgread.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)ccfgread.o $(MAKEFILE_DIR)ccfgread.o
		@ echo IAR: Compile chipinfo.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/chipinfo.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)chipinfo.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)chipinfo.o $(MAKEFILE_DIR)chipinfo.o
		@ echo IAR: Compile cpu.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/cpu.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)cpu.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)cpu.o $(MAKEFILE_DIR)cpu.o
		@ echo IAR: Compile ddi.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/ddi.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)ddi.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)ddi.o $(MAKEFILE_DIR)ddi.o
		@ echo IAR: Compile debug.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/debug.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)debug.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)debug.o $(MAKEFILE_DIR)debug.o
		@ echo IAR: Compile driverlib_release.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/driverlib_release.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)driverlib_release.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)driverlib_release.o $(MAKEFILE_DIR)driverlib_release.o
		@ echo IAR: Compile event.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/event.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)event.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)event.o $(MAKEFILE_DIR)event.o
		@ echo IAR: Compile flash.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/flash.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)flash.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)flash.o $(MAKEFILE_DIR)flash.o
		@ echo IAR: Compile gpio.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/gpio.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)gpio.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)gpio.o $(MAKEFILE_DIR)gpio.o
		@ echo IAR: Compile i2c.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/i2c.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)i2c.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)i2c.o $(MAKEFILE_DIR)i2c.o
		@ echo IAR: Compile i2s.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/i2s.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)i2s.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)i2s.o $(MAKEFILE_DIR)i2s.o
		@ echo IAR: Compile interrupt.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/interrupt.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)interrupt.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)interrupt.o $(MAKEFILE_DIR)interrupt.o
		@ echo IAR: Compile ioc.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/ioc.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)ioc.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)ioc.o $(MAKEFILE_DIR)ioc.o
		@ echo IAR: Compile osc.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/osc.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)osc.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)osc.o $(MAKEFILE_DIR)osc.o
		@ echo IAR: Compile pka.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/pka.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)pka.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)pka.o $(MAKEFILE_DIR)pka.o
		@ echo IAR: Compile prcm.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/prcm.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)prcm.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)prcm.o $(MAKEFILE_DIR)prcm.o
		@ echo IAR: Compile pwr_ctrl.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/pwr_ctrl.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)pwr_ctrl.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)pwr_ctrl.o $(MAKEFILE_DIR)pwr_ctrl.o
		@ echo IAR: Compile rom_crypto.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/rom_crypto.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)rom_crypto.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)rom_crypto.o $(MAKEFILE_DIR)rom_crypto.o
		@ echo IAR: Compile setup.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/setup.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)setup.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)setup.o $(MAKEFILE_DIR)setup.o
		@ echo IAR: Compile setup_rom.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/setup_rom.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)setup_rom.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)setup_rom.o $(MAKEFILE_DIR)setup_rom.o
		@ echo IAR: Compile sha2.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/sha2.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)sha2.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)sha2.o $(MAKEFILE_DIR)sha2.o
		@ echo IAR: Compile smph.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/smph.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)smph.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)smph.o $(MAKEFILE_DIR)smph.o
		@ echo IAR: Compile ssi.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/ssi.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)ssi.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)ssi.o $(MAKEFILE_DIR)ssi.o
		@ echo IAR: Compile sw_chacha.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/sw_chacha.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)sw_chacha.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)sw_chacha.o $(MAKEFILE_DIR)sw_chacha.o
		@ echo IAR: Compile sw_poly1305-donna.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/sw_poly1305-donna.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)sw_poly1305-donna.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)sw_poly1305-donna.o $(MAKEFILE_DIR)sw_poly1305-donna.o
		@ echo IAR: Compile systick.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/systick.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)systick.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)systick.o $(MAKEFILE_DIR)systick.o
		@ echo IAR: Compile sys_ctrl.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/sys_ctrl.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)sys_ctrl.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)sys_ctrl.o $(MAKEFILE_DIR)sys_ctrl.o
		@ echo IAR: Compile timer.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/timer.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)timer.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)timer.o $(MAKEFILE_DIR)timer.o
		@ echo IAR: Compile trng.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/trng.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)trng.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)trng.o $(MAKEFILE_DIR)trng.o
		@ echo IAR: Compile uart.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/uart.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)uart.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)uart.o $(MAKEFILE_DIR)uart.o
		@ echo IAR: Compile udma.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/udma.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)udma.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)udma.o $(MAKEFILE_DIR)udma.o
		@ echo IAR: Compile vims.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/vims.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)vims.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)vims.o $(MAKEFILE_DIR)vims.o
		@ echo IAR: Compile watchdog.c
		@ $(COMPILER_TOOL) $(MAKEFILE_DIR)../../../driverlib/watchdog.c -D nDEBUG $(ADD_PARAM) -o $(MAKEFILE_DIR)watchdog.o --no_clustering --debug --endian=little --cpu=Cortex-M4 -e --fpu=FPv4_sp -Ohz --require_prototypes --silent
		@ $(OBJ_MANIP_TOOL) --remove_file_path --remove_section ".comment" --silent $(MAKEFILE_DIR)watchdog.o $(MAKEFILE_DIR)watchdog.o
		@ echo IAR: Archive driverlib.lib
		@ $(ARCHIVER_TOOL) $(MAKEFILE_DIR)adi.o $(MAKEFILE_DIR)aes.o $(MAKEFILE_DIR)aon_batmon.o $(MAKEFILE_DIR)aon_event.o $(MAKEFILE_DIR)aon_ioc.o $(MAKEFILE_DIR)aon_pmctl.o $(MAKEFILE_DIR)aon_rtc.o $(MAKEFILE_DIR)aux_adc.o $(MAKEFILE_DIR)aux_dac.o $(MAKEFILE_DIR)aux_smph.o $(MAKEFILE_DIR)aux_sysif.o $(MAKEFILE_DIR)aux_tdc.o $(MAKEFILE_DIR)ccfgread.o $(MAKEFILE_DIR)chipinfo.o $(MAKEFILE_DIR)cpu.o $(MAKEFILE_DIR)ddi.o $(MAKEFILE_DIR)debug.o $(MAKEFILE_DIR)driverlib_release.o $(MAKEFILE_DIR)event.o $(MAKEFILE_DIR)flash.o $(MAKEFILE_DIR)gpio.o $(MAKEFILE_DIR)i2c.o $(MAKEFILE_DIR)i2s.o $(MAKEFILE_DIR)interrupt.o $(MAKEFILE_DIR)ioc.o $(MAKEFILE_DIR)osc.o $(MAKEFILE_DIR)pka.o $(MAKEFILE_DIR)prcm.o $(MAKEFILE_DIR)pwr_ctrl.o $(MAKEFILE_DIR)rom_crypto.o $(MAKEFILE_DIR)setup.o $(MAKEFILE_DIR)setup_rom.o $(MAKEFILE_DIR)sha2.o $(MAKEFILE_DIR)smph.o $(MAKEFILE_DIR)ssi.o $(MAKEFILE_DIR)sw_chacha.o $(MAKEFILE_DIR)sw_poly1305-donna.o $(MAKEFILE_DIR)systick.o $(MAKEFILE_DIR)sys_ctrl.o $(MAKEFILE_DIR)timer.o $(MAKEFILE_DIR)trng.o $(MAKEFILE_DIR)uart.o $(MAKEFILE_DIR)udma.o $(MAKEFILE_DIR)vims.o $(MAKEFILE_DIR)watchdog.o --create -o $(MAKEFILE_DIR)driverlib.lib
		@ rm -f $(MAKEFILE_DIR)*.o

# Deletes previous output and temporary files
clean :
		@ rm -fR $(MAKEFILE_DIR)*.o
		@ rm -fR $(MAKEFILE_DIR)*.lib
