################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include startup/subdir.mk
-include src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: Progetto\ Finale.elf

dependents:
	-cd C:/Users/Franco\ Bressan/workspace/LabArch/stm32f401c-disco_stdperiph_lib/Debug && $(MAKE) all

# Tool invocations
Progetto\ Finale.elf: $(OBJS) $(USER_OBJS) C:/Users/Franco\ Bressan/workspace/LabArch/stm32f401c-disco_stdperiph_lib/Debug/libstm32f401c-disco_stdperiph_lib.a
	@echo 'Building target: $@'
	@echo 'Invoking: MCU GCC Linker'
	arm-none-eabi-gcc -mcpu=cortex-m4 -mthumb -L"C:\Users\Franco Bressan\workspace\LabArch\stm32f401c-disco_stdperiph_lib\Debug" -T"C:\Users\Franco Bressan\workspace\LabArch\Progetto Finale\LinkerScript.ld" -Wl,-Map=output.map -Wl,--gc-sections -o "Progetto Finale.elf" $(OBJS) $(USER_OBJS) $(LIBS)
	@echo 'Finished building target: $@'
	@echo ' '
	$(MAKE) --no-print-directory post-build

# Other Targets
clean:
	-$(RM) *
	-@echo ' '

post-build:
	-@echo 'Generating binary:'
	-arm-none-eabi-objcopy -O binary "Progetto Finale.elf" "Progetto Finale.bin"
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY: post-build
C:/Users/Franco\ Bressan/workspace/LabArch/stm32f401c-disco_stdperiph_lib/Debug/libstm32f401c-disco_stdperiph_lib.a:

-include ../makefile.targets
