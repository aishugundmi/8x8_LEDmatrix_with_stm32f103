################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Drivers/STM32F1xx_HAL_Driver/Src/subdir.mk
-include Core/Startup/subdir.mk
-include Core/Src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
11\ 8x8_LEDmatrix_with_stm32f103.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
11\ 8x8_LEDmatrix_with_stm32f103.list \

OBJCOPY_BIN += \
11\ 8x8_LEDmatrix_with_stm32f103.bin \


# All Target
all: 11\ 8x8_LEDmatrix_with_stm32f103.elf secondary-outputs

# Tool invocations
11\ 8x8_LEDmatrix_with_stm32f103.elf: $(OBJS) $(USER_OBJS) C:\Users\Aishwarya\Desktop\stm\11\ 8x8_LEDmatrix_with_stm32f103\STM32F103C8TX_FLASH.ld
	arm-none-eabi-gcc -o "11 8x8_LEDmatrix_with_stm32f103.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m3 -T"C:\Users\Aishwarya\Desktop\stm\11 8x8_LEDmatrix_with_stm32f103\STM32F103C8TX_FLASH.ld" --specs=nosys.specs -Wl,-Map="11 8x8_LEDmatrix_with_stm32f103.map" -Wl,--gc-sections -static --specs=nano.specs -mfloat-abi=soft -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

11\ 8x8_LEDmatrix_with_stm32f103.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "11 8x8_LEDmatrix_with_stm32f103.list"
	@echo 'Finished building: $@'
	@echo ' '

11\ 8x8_LEDmatrix_with_stm32f103.bin: $(EXECUTABLES)
	arm-none-eabi-objcopy  -O binary $(EXECUTABLES) "11 8x8_LEDmatrix_with_stm32f103.bin"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) *
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST) $(OBJCOPY_BIN)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
