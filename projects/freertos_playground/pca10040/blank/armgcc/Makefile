PROJECT_NAME     := template_pca10040
TARGETS          := nrf52832_xxaa
OUTPUT_DIRECTORY := _build

SDK_ROOT := ../../../src
PROJ_DIR := ../../..

$(OUTPUT_DIRECTORY)/nrf52832_xxaa.out: \
  LINKER_SCRIPT  := template_gcc_nrf52.ld

# Source files common to all targets
SRC_FILES += \
  $(SDK_ROOT)/modules/nrfx/mdk/gcc_startup_nrf52.S \
  $(SDK_ROOT)/external/thedotfactory_fonts/orkney24pts.c \
  $(SDK_ROOT)/external/thedotfactory_fonts/orkney8pts.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/nrf_hw/nrf_hw_backend_init.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/nrf_hw/nrf_hw_backend_rng.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/nrf_hw/nrf_hw_backend_rng_mbedtls.c \
  $(SDK_ROOT)/components/boards/boards.c \
  $(SDK_ROOT)/components/libraries/mpu/nrf_mpu_lib.c \
  $(SDK_ROOT)/components/libraries/stack_guard/nrf_stack_guard.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/micro_ecc/micro_ecc_backend_ecc.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/micro_ecc/micro_ecc_backend_ecdh.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/micro_ecc/micro_ecc_backend_ecdsa.c \
  $(SDK_ROOT)/components/libraries/twi_sensor/nrf_twi_sensor.c \
  $(SDK_ROOT)/components/libraries/button/app_button.c \
  $(SDK_ROOT)/components/libraries/util/app_error.c \
  $(SDK_ROOT)/components/libraries/util/app_error_handler_gcc.c \
  $(SDK_ROOT)/components/libraries/util/app_error_weak.c \
  $(SDK_ROOT)/components/libraries/fifo/app_fifo.c \
  $(SDK_ROOT)/components/libraries/gpiote/app_gpiote.c \
  $(SDK_ROOT)/components/libraries/pwm/app_pwm.c \
  $(SDK_ROOT)/components/libraries/scheduler/app_scheduler.c \
  $(SDK_ROOT)/components/libraries/sdcard/app_sdcard.c \
  $(SDK_ROOT)/components/libraries/timer/app_timer2.c \
  $(SDK_ROOT)/components/libraries/uart/app_uart_fifo.c \
  $(SDK_ROOT)/components/libraries/util/app_util_platform.c \
  $(SDK_ROOT)/external/cifra_AES128-EAX/blockwise.c \
  $(SDK_ROOT)/external/cifra_AES128-EAX/cifra_cmac.c \
  $(SDK_ROOT)/external/cifra_AES128-EAX/cifra_eax_aes.c \
  $(SDK_ROOT)/components/libraries/crc16/crc16.c \
  $(SDK_ROOT)/components/libraries/crc32/crc32.c \
  $(SDK_ROOT)/external/cifra_AES128-EAX/eax.c \
  $(SDK_ROOT)/components/libraries/fds/fds.c \
  $(SDK_ROOT)/external/fnmatch/fnmatch.c \
  $(SDK_ROOT)/external/cifra_AES128-EAX/gf128.c \
  $(SDK_ROOT)/components/libraries/hardfault/nrf52/handler/hardfault_handler_gcc.c \
  $(SDK_ROOT)/components/libraries/hardfault/hardfault_implementation.c \
  $(SDK_ROOT)/components/libraries/hci/hci_mem_pool.c \
  $(SDK_ROOT)/components/libraries/hci/hci_slip.c \
  $(SDK_ROOT)/components/libraries/hci/hci_transport.c \
  $(SDK_ROOT)/components/libraries/led_softblink/led_softblink.c \
  $(SDK_ROOT)/components/libraries/low_power_pwm/low_power_pwm.c \
  $(SDK_ROOT)/components/libraries/mem_manager/mem_manager.c \
  $(SDK_ROOT)/external/cifra_AES128-EAX/modes.c \
  $(SDK_ROOT)/components/libraries/util/nrf_assert.c \
  $(SDK_ROOT)/components/libraries/atomic_fifo/nrf_atfifo.c \
  $(SDK_ROOT)/components/libraries/atomic/nrf_atomic.c \
  $(SDK_ROOT)/components/libraries/balloc/nrf_balloc.c \
  $(SDK_ROOT)/components/libraries/cli/nrf_cli.c \
  $(SDK_ROOT)/components/libraries/cli/uart/nrf_cli_uart.c \
  $(SDK_ROOT)/components/libraries/csense/nrf_csense.c \
  $(SDK_ROOT)/components/libraries/csense_drv/nrf_drv_csense.c \
  $(SDK_ROOT)/external/fprintf/nrf_fprintf.c \
  $(SDK_ROOT)/external/fprintf/nrf_fprintf_format.c \
  $(SDK_ROOT)/components/libraries/fstorage/nrf_fstorage.c \
  $(SDK_ROOT)/components/libraries/fstorage/nrf_fstorage_nvmc.c \
  $(SDK_ROOT)/components/libraries/gfx/nrf_gfx.c \
  $(SDK_ROOT)/components/libraries/memobj/nrf_memobj.c \
  $(SDK_ROOT)/components/libraries/pwr_mgmt/nrf_pwr_mgmt.c \
  $(SDK_ROOT)/components/libraries/queue/nrf_queue.c \
  $(SDK_ROOT)/components/libraries/ringbuf/nrf_ringbuf.c \
  $(SDK_ROOT)/components/libraries/experimental_section_vars/nrf_section_iter.c \
  $(SDK_ROOT)/components/libraries/sortlist/nrf_sortlist.c \
  $(SDK_ROOT)/components/libraries/spi_mngr/nrf_spi_mngr.c \
  $(SDK_ROOT)/components/libraries/strerror/nrf_strerror.c \
  $(SDK_ROOT)/components/libraries/twi_mngr/nrf_twi_mngr.c \
  $(SDK_ROOT)/components/libraries/slip/slip.c \
  $(SDK_ROOT)/components/libraries/experimental_task_manager/task_manager.c \
  $(SDK_ROOT)/components/libraries/experimental_task_manager/task_manager_core_armgcc.S \
  $(SDK_ROOT)/components/libraries/crypto/backend/mbedtls/mbedtls_backend_aes.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/mbedtls/mbedtls_backend_aes_aead.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/mbedtls/mbedtls_backend_ecc.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/mbedtls/mbedtls_backend_ecdh.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/mbedtls/mbedtls_backend_ecdsa.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/mbedtls/mbedtls_backend_hash.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/mbedtls/mbedtls_backend_hmac.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/mbedtls/mbedtls_backend_init.c \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_frontend.c \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_str_formatter.c \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_default_backends.c \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_backend_serial.c \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_backend_uart.c \
  $(SDK_ROOT)/integration/nrfx/legacy/nrf_drv_clock.c \
  $(SDK_ROOT)/integration/nrfx/legacy/nrf_drv_power.c \
  $(SDK_ROOT)/integration/nrfx/legacy/nrf_drv_ppi.c \
  $(SDK_ROOT)/integration/nrfx/legacy/nrf_drv_rng.c \
  $(SDK_ROOT)/integration/nrfx/legacy/nrf_drv_spi.c \
  $(SDK_ROOT)/integration/nrfx/legacy/nrf_drv_spis.c \
  $(SDK_ROOT)/integration/nrfx/legacy/nrf_drv_swi.c \
  $(SDK_ROOT)/integration/nrfx/legacy/nrf_drv_twi.c \
  $(SDK_ROOT)/integration/nrfx/legacy/nrf_drv_uart.c \
  $(SDK_ROOT)/components/drivers_nrf/nrf_soc_nosd/nrf_nvic.c \
  $(SDK_ROOT)/modules/nrfx/hal/nrf_nvmc.c \
  $(SDK_ROOT)/components/drivers_nrf/nrf_soc_nosd/nrf_soc.c \
  $(SDK_ROOT)/modules/nrfx/soc/nrfx_atomic.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_clock.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_comp.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_gpiote.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_i2s.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_lpcomp.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_pdm.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_power.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_ppi.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/prs/nrfx_prs.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_pwm.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_qdec.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_rng.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_rtc.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_saadc.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_spi.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_spim.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_spis.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_swi.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_systick.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_timer.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_twi.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_twim.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_twis.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_uart.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_uarte.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_wdt.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_aead.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_aes.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_aes_shared.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_ecc.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_ecdh.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_ecdsa.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_eddsa.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_error.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_hash.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_hkdf.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_hmac.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_init.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_rng.c \
  $(SDK_ROOT)/components/libraries/crypto/nrf_crypto_shared.c \
  $(PROJ_DIR)/main.c \
  $(SDK_ROOT)/external/mbedtls/library/aes.c \
  $(SDK_ROOT)/external/mbedtls/library/aesni.c \
  $(SDK_ROOT)/external/mbedtls/library/arc4.c \
  $(SDK_ROOT)/external/mbedtls/library/aria.c \
  $(SDK_ROOT)/external/mbedtls/library/asn1parse.c \
  $(SDK_ROOT)/external/mbedtls/library/asn1write.c \
  $(SDK_ROOT)/external/mbedtls/library/base64.c \
  $(SDK_ROOT)/external/mbedtls/library/bignum.c \
  $(SDK_ROOT)/external/mbedtls/library/blowfish.c \
  $(SDK_ROOT)/external/mbedtls/library/camellia.c \
  $(SDK_ROOT)/external/mbedtls/library/ccm.c \
  $(SDK_ROOT)/external/mbedtls/library/certs.c \
  $(SDK_ROOT)/external/mbedtls/library/chacha20.c \
  $(SDK_ROOT)/external/mbedtls/library/chachapoly.c \
  $(SDK_ROOT)/external/mbedtls/library/cipher.c \
  $(SDK_ROOT)/external/mbedtls/library/cipher_wrap.c \
  $(SDK_ROOT)/external/mbedtls/library/cmac.c \
  $(SDK_ROOT)/external/mbedtls/library/ctr_drbg.c \
  $(SDK_ROOT)/external/mbedtls/library/debug.c \
  $(SDK_ROOT)/external/mbedtls/library/des.c \
  $(SDK_ROOT)/external/mbedtls/library/dhm.c \
  $(SDK_ROOT)/external/mbedtls/library/ecdh.c \
  $(SDK_ROOT)/external/mbedtls/library/ecdsa.c \
  $(SDK_ROOT)/external/mbedtls/library/ecjpake.c \
  $(SDK_ROOT)/external/mbedtls/library/ecp.c \
  $(SDK_ROOT)/external/mbedtls/library/ecp_curves.c \
  $(SDK_ROOT)/external/mbedtls/library/entropy.c \
  $(SDK_ROOT)/external/mbedtls/library/entropy_poll.c \
  $(SDK_ROOT)/external/mbedtls/library/error.c \
  $(SDK_ROOT)/external/mbedtls/library/gcm.c \
  $(SDK_ROOT)/external/mbedtls/library/havege.c \
  $(SDK_ROOT)/external/mbedtls/library/hmac_drbg.c \
  $(SDK_ROOT)/external/mbedtls/library/md.c \
  $(SDK_ROOT)/external/mbedtls/library/md2.c \
  $(SDK_ROOT)/external/mbedtls/library/md4.c \
  $(SDK_ROOT)/external/mbedtls/library/md5.c \
  $(SDK_ROOT)/external/mbedtls/library/md_wrap.c \
  $(SDK_ROOT)/external/mbedtls/library/memory_buffer_alloc.c \
  $(SDK_ROOT)/external/mbedtls/library/net_sockets.c \
  $(SDK_ROOT)/external/mbedtls/library/nist_kw.c \
  $(SDK_ROOT)/external/mbedtls/library/oid.c \
  $(SDK_ROOT)/external/mbedtls/library/padlock.c \
  $(SDK_ROOT)/external/mbedtls/library/pem.c \
  $(SDK_ROOT)/external/mbedtls/library/pk.c \
  $(SDK_ROOT)/external/mbedtls/library/pk_wrap.c \
  $(SDK_ROOT)/external/mbedtls/library/pkcs11.c \
  $(SDK_ROOT)/external/mbedtls/library/pkcs12.c \
  $(SDK_ROOT)/external/mbedtls/library/pkcs5.c \
  $(SDK_ROOT)/external/mbedtls/library/pkparse.c \
  $(SDK_ROOT)/external/mbedtls/library/pkwrite.c \
  $(SDK_ROOT)/external/mbedtls/library/platform.c \
  $(SDK_ROOT)/external/mbedtls/library/platform_util.c \
  $(SDK_ROOT)/external/mbedtls/library/poly1305.c \
  $(SDK_ROOT)/external/mbedtls/library/ripemd160.c \
  $(SDK_ROOT)/external/mbedtls/library/rsa.c \
  $(SDK_ROOT)/external/mbedtls/library/rsa_internal.c \
  $(SDK_ROOT)/external/mbedtls/library/sha1.c \
  $(SDK_ROOT)/external/mbedtls/library/sha256.c \
  $(SDK_ROOT)/external/mbedtls/library/sha512.c \
  $(SDK_ROOT)/external/mbedtls/library/ssl_cache.c \
  $(SDK_ROOT)/external/mbedtls/library/ssl_ciphersuites.c \
  $(SDK_ROOT)/external/mbedtls/library/ssl_cli.c \
  $(SDK_ROOT)/external/mbedtls/library/ssl_cookie.c \
  $(SDK_ROOT)/external/mbedtls/library/ssl_srv.c \
  $(SDK_ROOT)/external/mbedtls/library/ssl_ticket.c \
  $(SDK_ROOT)/external/mbedtls/library/ssl_tls.c \
  $(SDK_ROOT)/external/mbedtls/library/threading.c \
  $(SDK_ROOT)/external/mbedtls/library/version.c \
  $(SDK_ROOT)/external/mbedtls/library/version_features.c \
  $(SDK_ROOT)/external/mbedtls/library/x509.c \
  $(SDK_ROOT)/external/mbedtls/library/x509_create.c \
  $(SDK_ROOT)/external/mbedtls/library/x509_crl.c \
  $(SDK_ROOT)/external/mbedtls/library/x509_crt.c \
  $(SDK_ROOT)/external/mbedtls/library/x509_csr.c \
  $(SDK_ROOT)/external/mbedtls/library/x509write_crt.c \
  $(SDK_ROOT)/external/mbedtls/library/x509write_csr.c \
  $(SDK_ROOT)/external/mbedtls/library/xtea.c \
  $(SDK_ROOT)/modules/nrfx/mdk/system_nrf52.c \
  $(SDK_ROOT)/components/libraries/bsp/bsp.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/cifra/cifra_backend_aes_aead.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/oberon/oberon_backend_chacha_poly_aead.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/oberon/oberon_backend_ecc.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/oberon/oberon_backend_ecdh.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/oberon/oberon_backend_ecdsa.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/oberon/oberon_backend_eddsa.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/oberon/oberon_backend_hash.c \
  $(SDK_ROOT)/components/libraries/crypto/backend/oberon/oberon_backend_hmac.c \
  $(SDK_ROOT)/external/freertos/source/croutine.c \
  $(SDK_ROOT)/external/freertos/source/event_groups.c \
  $(SDK_ROOT)/external/freertos/source/portable/MemMang/heap_1.c \
  $(SDK_ROOT)/external/freertos/source/list.c \
  $(SDK_ROOT)/external/freertos/portable/GCC/nrf52/port.c \
  $(SDK_ROOT)/external/freertos/portable/CMSIS/nrf52/port_cmsis.c \
  $(SDK_ROOT)/external/freertos/portable/CMSIS/nrf52/port_cmsis_systick.c \
  $(SDK_ROOT)/external/freertos/source/queue.c \
  $(SDK_ROOT)/external/freertos/source/stream_buffer.c \
  $(SDK_ROOT)/external/freertos/source/tasks.c \
  $(SDK_ROOT)/external/freertos/source/timers.c \
  $(SDK_ROOT)/integration/nrfx/legacy/nrf_drv_clock.c \

# Include folders common to all targets
INC_FOLDERS += \
  $(SDK_ROOT)/components \
  $(SDK_ROOT)/components/libraries/cli \
  $(SDK_ROOT)/modules/nrfx/mdk \
  $(SDK_ROOT)/external/nrf_cc310/include \
  $(SDK_ROOT)/components/libraries/scheduler \
  $(SDK_ROOT)/modules/nrfx \
  $(SDK_ROOT)/components/libraries/slip \
  $(SDK_ROOT)/components/libraries/crypto/backend/oberon \
  $(SDK_ROOT)/components/libraries/queue \
  $(SDK_ROOT)/components/libraries/pwr_mgmt \
  $(SDK_ROOT)/components/libraries/fifo \
  $(SDK_ROOT)/components/libraries/sortlist \
  $(SDK_ROOT)/components/libraries/strerror \
  $(SDK_ROOT)/components/libraries/pwm \
  $(SDK_ROOT)/components/libraries/crc32 \
  $(SDK_ROOT)/integration/nrfx/legacy \
  $(SDK_ROOT)/components/libraries/crc16 \
  $(SDK_ROOT)/components/libraries/mem_manager \
  $(SDK_ROOT)/components/toolchain/cmsis/include \
  $(SDK_ROOT)/components/libraries/crypto/backend/optiga \
  $(SDK_ROOT)/components/libraries/crypto/backend/mbedtls \
  ../config \
  $(SDK_ROOT)/components/libraries/csense_drv \
  $(SDK_ROOT)/components/libraries/crypto \
  $(SDK_ROOT)/components/libraries/crypto/backend/nrf_sw \
  $(SDK_ROOT)/components/libraries/ecc \
  $(SDK_ROOT)/components/libraries/ringbuf \
  $(SDK_ROOT)/components/libraries/stack_guard \
  $(SDK_ROOT)/components/libraries/hardfault/nrf52 \
  $(SDK_ROOT)/components/libraries/cli/uart \
  $(SDK_ROOT)/components/libraries/bsp \
  $(SDK_ROOT)/components/libraries/crypto/backend/cc310 \
  $(SDK_ROOT)/external/nrf_oberon \
  $(SDK_ROOT)/external/micro-ecc/micro-ecc \
  $(SDK_ROOT)/components/libraries/uart \
  $(SDK_ROOT)/components/libraries/crypto/backend/nrf_hw \
  $(SDK_ROOT)/components/libraries/hci \
  $(SDK_ROOT)/components/libraries/log \
  $(SDK_ROOT)/components/libraries/gpiote \
  $(SDK_ROOT)/components/libraries/button \
  $(SDK_ROOT)/components/libraries/mpu \
  $(SDK_ROOT)/components/libraries/fstorage \
  $(SDK_ROOT)/components/libraries/experimental_section_vars \
  $(SDK_ROOT)/components/libraries/twi_sensor \
  $(SDK_ROOT)/components/libraries/util \
  $(SDK_ROOT)/external/cifra_AES128-EAX \
  $(SDK_ROOT)/external/mbedtls/include \
  $(SDK_ROOT)/external/protothreads/pt-1.4 \
  $(SDK_ROOT)/components/libraries/mutex \
  $(PROJ_DIR) \
  $(SDK_ROOT)/components/libraries/gfx \
  $(SDK_ROOT)/components/libraries/delay \
  $(SDK_ROOT)/external/nrf_oberon/include \
  $(SDK_ROOT)/components/libraries/atomic_fifo \
  $(SDK_ROOT)/components/drivers_nrf/nrf_soc_nosd \
  $(SDK_ROOT)/components/libraries/atomic \
  $(SDK_ROOT)/components/boards \
  $(SDK_ROOT)/external/nrf_tls/mbedtls/nrf_crypto/config \
  $(SDK_ROOT)/external/protothreads \
  $(SDK_ROOT)/components/libraries/spi_mngr \
  $(SDK_ROOT)/components/libraries/memobj \
  $(SDK_ROOT)/components/libraries/crypto/backend/cc310_bl \
  $(SDK_ROOT)/components/libraries/csense \
  $(SDK_ROOT)/external/fnmatch \
  $(SDK_ROOT)/integration/nrfx \
  $(SDK_ROOT)/components/libraries/fds \
  $(SDK_ROOT)/components/libraries/twi_mngr \
  $(SDK_ROOT)/external/thedotfactory_fonts \
  $(SDK_ROOT)/components/libraries/balloc \
  $(SDK_ROOT)/components/libraries/hardfault \
  $(SDK_ROOT)/components/libraries/stack_info \
  $(SDK_ROOT)/components/libraries/crypto/backend/micro_ecc \
  $(SDK_ROOT)/components/libraries/crypto/backend/cifra \
  $(SDK_ROOT)/components/libraries/led_softblink \
  $(SDK_ROOT)/modules/nrfx/drivers/include \
  $(SDK_ROOT)/components/libraries/experimental_task_manager \
  $(SDK_ROOT)/components/libraries/low_power_pwm \
  $(SDK_ROOT)/components/libraries/timer \
  $(SDK_ROOT)/modules/nrfx/hal \
  $(SDK_ROOT)/external/fprintf \
  $(SDK_ROOT)/components/libraries/sdcard \
  $(SDK_ROOT)/components/libraries/log/src \
  $(PROJ_DIR)/config \
  $(SDK_ROOT)/external/freertos/source/include \
  $(SDK_ROOT)/external/freertos/config \
  $(SDK_ROOT)/external/freertos/portable/CMSIS/nrf52 \
  $(SDK_ROOT)/external/freertos/portable/GCC/nrf52 \
  $(SDK_ROOT)/integration/nrfx/legacy \

#LIB_FILES += \
#  $(SDK_ROOT)/external/nrf_cc310/lib/cortex-m4/hard-float/libnrf_cc310_0.9.13.a \
#  $(SDK_ROOT)/external/micro-ecc/nrf52hf_armgcc/armgcc/micro_ecc_lib_nrf52.a \
#  $(SDK_ROOT)/external/nrf_oberon/lib/cortex-m4/hard-float/liboberon_3.0.8.a \

# Optimization flags
OPT = -O3 -g3
# Uncomment the line below to enable link time optimization
#OPT += -flto

# C flags common to all targets
CFLAGS += $(OPT)
CFLAGS += -DAPP_TIMER_V2
CFLAGS += -DAPP_TIMER_V2_RTC1_ENABLED
CFLAGS += -DBOARD_PCA10040
CFLAGS += -DCONFIG_GPIO_AS_PINRESET
CFLAGS += -DFLOAT_ABI_HARD
CFLAGS += -DMBEDTLS_CONFIG_FILE=\"nrf_crypto_mbedtls_config.h\"
CFLAGS += -DNRF52
CFLAGS += -DNRF52832_XXAA
CFLAGS += -DNRF52_PAN_74
CFLAGS += -DNRF_CRYPTO_MAX_INSTANCE_COUNT=1
CFLAGS += -DuECC_ENABLE_VLI_API=0
CFLAGS += -DuECC_OPTIMIZATION_LEVEL=3
CFLAGS += -DuECC_SQUARE_FUNC=0
CFLAGS += -DuECC_SUPPORT_COMPRESSED_POINT=0
CFLAGS += -DuECC_VLI_NATIVE_LITTLE_ENDIAN=1
CFLAGS += -mcpu=cortex-m4
CFLAGS += -mthumb -mabi=aapcs
CFLAGS += -Wall -Werror
CFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
# keep every function in a separate section, this allows linker to discard unused ones
CFLAGS += -ffunction-sections -fdata-sections -fno-strict-aliasing
CFLAGS += -fno-builtin -fshort-enums

# C++ flags common to all targets
CXXFLAGS += $(OPT)
# Assembler flags common to all targets
ASMFLAGS += -g3
ASMFLAGS += -mcpu=cortex-m4
ASMFLAGS += -mthumb -mabi=aapcs
ASMFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
ASMFLAGS += -DAPP_TIMER_V2
ASMFLAGS += -DAPP_TIMER_V2_RTC1_ENABLED
ASMFLAGS += -DBOARD_PCA10040
ASMFLAGS += -DCONFIG_GPIO_AS_PINRESET
ASMFLAGS += -DFLOAT_ABI_HARD
ASMFLAGS += -DNRF52
ASMFLAGS += -DNRF52832_XXAA
ASMFLAGS += -DNRF52_PAN_74
ASMFLAGS += -DNRF_CRYPTO_MAX_INSTANCE_COUNT=1
ASMFLAGS += -DuECC_ENABLE_VLI_API=0
ASMFLAGS += -DuECC_OPTIMIZATION_LEVEL=3
ASMFLAGS += -DuECC_SQUARE_FUNC=0
ASMFLAGS += -DuECC_SUPPORT_COMPRESSED_POINT=0
ASMFLAGS += -DuECC_VLI_NATIVE_LITTLE_ENDIAN=1

# Linker flags
LDFLAGS += $(OPT)
LDFLAGS += -mthumb -mabi=aapcs -L$(SDK_ROOT)/modules/nrfx/mdk -T$(LINKER_SCRIPT)
LDFLAGS += -mcpu=cortex-m4
LDFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
# let linker dump unused sections
LDFLAGS += -Wl,--gc-sections
# use newlib in nano version
LDFLAGS += --specs=nano.specs

nrf52832_xxaa: CFLAGS += -D__HEAP_SIZE=8192
nrf52832_xxaa: CFLAGS += -D__STACK_SIZE=8192
nrf52832_xxaa: ASMFLAGS += -D__HEAP_SIZE=8192
nrf52832_xxaa: ASMFLAGS += -D__STACK_SIZE=8192

# Add standard libraries at the very end of the linker input, after all objects
# that may need symbols provided by these libraries.
LIB_FILES += -lc -lnosys -lm


.PHONY: default help

# Default target - first one defined
default: nrf52832_xxaa

# Print all targets that can be built
help:
	@echo following targets are available:
	@echo		nrf52832_xxaa
	@echo		sdk_config - starting external tool for editing sdk_config.h
	@echo		flash      - flashing binary

TEMPLATE_PATH := $(SDK_ROOT)/components/toolchain/gcc


include $(TEMPLATE_PATH)/Makefile.common

$(foreach target, $(TARGETS), $(call define_target, $(target)))

.PHONY: flash erase

# Flash the program
flash:
	@echo Flashing: $(OUTPUT_DIRECTORY)/nrf52832_xxaa.hex
	sudo openocd -f interface/stlink.cfg -f target/nrf52.cfg -c "init; reset halt; nrf5 mass_erase; program _build/nrf52832_xxaa.hex; reset; exit;"

erase:
	nrfjprog -f nrf52 --eraseall

SDK_CONFIG_FILE := ../config/sdk_config.h
CMSIS_CONFIG_TOOL := $(SDK_ROOT)/external_tools/cmsisconfig/CMSIS_Configuration_Wizard.jar
sdk_config:
	java -jar $(CMSIS_CONFIG_TOOL) $(SDK_CONFIG_FILE)
