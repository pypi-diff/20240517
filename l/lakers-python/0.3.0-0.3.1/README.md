# Comparing `tmp/lakers_python-0.3.0.tar.gz` & `tmp/lakers_python-0.3.1.tar.gz`

## Comparing `lakers_python-0.3.0.tar` & `lakers_python-0.3.1.tar`

### file list

```diff
@@ -1,149 +1,159 @@
--rw-r--r--   0   671610   202045      384 2024-01-16 08:08:59.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/Cargo.toml
--rw-r--r--   0   671610   202045     1580 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/build.rs
--rw-r--r--   0   671610   202045     2050 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/src/c/wrapper.h
--rw-r--r--   0   671610   202045    10187 2024-04-05 13:22:30.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/src/lib.rs
--rw-r--r--   0   671610   202045      771 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile
--rw-r--r--   0   671610   202045     1217 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile.internal
--rw-r--r--   0   671610   202045     4213 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_defs.h
--rw-r--r--   0   671610   202045     4680 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_utils.c
--rw-r--r--   0   671610   202045    13789 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_data.h
--rw-r--r--   0   671610   202045     3989 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_defs.h
--rw-r--r--   0   671610   202045     6951 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ccsw_crys_rsa_shared_types.h
--rw-r--r--   0   671610   202045    18924 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm.h
--rw-r--r--   0   671610   202045     7180 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm_error.h
--rw-r--r--   0   671610   202045    12210 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha.h
--rw-r--r--   0   671610   202045     5299 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_error.h
--rw-r--r--   0   671610   202045     5336 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly.h
--rw-r--r--   0   671610   202045     4848 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly_error.h
--rw-r--r--   0   671610   202045    17291 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common.h
--rw-r--r--   0   671610   202045     5103 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common_error.h
--rw-r--r--   0   671610   202045    28262 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh.h
--rw-r--r--   0   671610   202045     8030 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_error.h
--rw-r--r--   0   671610   202045    12591 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_kg.h
--rw-r--r--   0   671610   202045    11841 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_edw_api.h
--rw-r--r--   0   671610   202045    13273 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_api.h
--rw-r--r--   0   671610   202045     6273 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_edw_error.h
--rw-r--r--   0   671610   202045    13454 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_build.h
--rw-r--r--   0   671610   202045     5126 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_dh.h
--rw-r--r--   0   671610   202045     3832 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_domain.h
--rw-r--r--   0   671610   202045     8772 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_ecdsa.h
--rw-r--r--   0   671610   202045    19639 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_error.h
--rw-r--r--   0   671610   202045     4757 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_kg.h
--rw-r--r--   0   671610   202045    19193 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_types.h
--rw-r--r--   0   671610   202045    12890 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_error.h
--rw-r--r--   0   671610   202045    13780 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash.h
--rw-r--r--   0   671610   202045     3376 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_defs.h
--rw-r--r--   0   671610   202045     5101 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_error.h
--rw-r--r--   0   671610   202045     6138 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf.h
--rw-r--r--   0   671610   202045     4247 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf_error.h
--rw-r--r--   0   671610   202045    11821 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac.h
--rw-r--r--   0   671610   202045     3374 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_defs.h
--rw-r--r--   0   671610   202045     5259 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_error.h
--rw-r--r--   0   671610   202045    10891 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf.h
--rw-r--r--   0   671610   202045     5154 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf_error.h
--rw-r--r--   0   671610   202045     7450 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_pka_defs_hw.h
--rw-r--r--   0   671610   202045     4998 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly.h
--rw-r--r--   0   671610   202045     4170 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly_error.h
--rw-r--r--   0   671610   202045    19714 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd.h
--rw-r--r--   0   671610   202045     8213 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd_error.h
--rw-r--r--   0   671610   202045     9721 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_build.h
--rw-r--r--   0   671610   202045    16219 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_error.h
--rw-r--r--   0   671610   202045     7582 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_kg.h
--rw-r--r--   0   671610   202045     7921 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_prim.h
--rw-r--r--   0   671610   202045    34649 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_schemes.h
--rw-r--r--   0   671610   202045    23132 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_types.h
--rw-r--r--   0   671610   202045    17872 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp.h
--rw-r--r--   0   671610   202045     4401 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp_error.h
--rw-r--r--   0   671610   202045     3641 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/dx_reg_base_host.h
--rw-r--r--   0   671610   202045     4914 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/sns_silib.h
--rw-r--r--   0   671610   202045    17381 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes.h
--rw-r--r--   0   671610   202045     4168 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_defs.h
--rw-r--r--   0   671610   202045     7180 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_error.h
--rw-r--r--   0   671610   202045     4233 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_bitops.h
--rw-r--r--   0   671610   202045     3536 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_abort.h
--rw-r--r--   0   671610   202045     3700 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_barrier.h
--rw-r--r--   0   671610   202045     8494 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_compiler.h
--rw-r--r--   0   671610   202045     9900 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma.h
--rw-r--r--   0   671610   202045     4089 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_defs.h
--rw-r--r--   0   671610   202045     3582 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_plat.h
--rw-r--r--   0   671610   202045     4187 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_error.h
--rw-r--r--   0   671610   202045     9241 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file.h
--rw-r--r--   0   671610   202045     5012 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file_plat.h
--rw-r--r--   0   671610   202045     4816 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_fips.h
--rw-r--r--   0   671610   202045     4021 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_init.h
--rw-r--r--   0   671610   202045     4605 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_list.h
--rw-r--r--   0   671610   202045     9188 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_log.h
--rw-r--r--   0   671610   202045     7156 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mem.h
--rw-r--r--   0   671610   202045     4487 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_memmap.h
--rw-r--r--   0   671610   202045     5729 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex.h
--rw-r--r--   0   671610   202045     3606 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex_plat.h
--rw-r--r--   0   671610   202045     5696 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf.h
--rw-r--r--   0   671610   202045     3287 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf_plat.h
--rw-r--r--   0   671610   202045     5074 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem.h
--rw-r--r--   0   671610   202045     5028 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem_plat.h
--rw-r--r--   0   671610   202045     3426 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_trng.h
--rw-r--r--   0   671610   202045     5532 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types.h
--rw-r--r--   0   671610   202045     3458 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types_plat.h
--rw-r--r--   0   671610   202045     3885 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pka_hw_plat_defs.h
--rw-r--r--   0   671610   202045     8745 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_regs.h
--rw-r--r--   0   671610   202045     3742 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_sram_map.h
--rw-r--r--   0   671610   202045     4544 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_defs.h
--rw-r--r--   0   671610   202045     5141 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_error.h
--rw-r--r--   0   671610   202045     5670 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation.h
--rw-r--r--   0   671610   202045     4277 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation_defs.h
--rw-r--r--   0   671610   202045   297096 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/libnrf_cc310_0.9.13.a
--rw-r--r--   0   671610   202045   296510 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/no-interrupts/libnrf_cc310_0.9.13.a
--rw-r--r--   0   671610   202045   297096 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/libnrf_cc310_0.9.13.a
--rw-r--r--   0   671610   202045   296510 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a
--rw-r--r--   0   671610   202045   296510 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib
--rw-r--r--   0   671610   202045   297096 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/nrf_cc310_0.9.13.lib
--rw-r--r--   0   671610   202045   295748 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/libnrf_cc310_0.9.13.a
--rw-r--r--   0   671610   202045   295162 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/no-interrupts/libnrf_cc310_0.9.13.a
--rw-r--r--   0   671610   202045   295748 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/libnrf_cc310_0.9.13.a
--rw-r--r--   0   671610   202045   295162 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a
--rw-r--r--   0   671610   202045   295162 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib
--rw-r--r--   0   671610   202045   295748 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/nrf_cc310_0.9.13.lib
--rw-r--r--   0   671610   202045     1501 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/license.txt
--rw-r--r--   0   671610   202045     1501 2023-12-13 09:05:23.000000 lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/license.txt
--rw-r--r--   0   671610   202045      136 2024-01-16 08:08:59.000000 lakers_python-0.3.0/shared/README.md
--rw-r--r--   0   671610   202045      753 2024-01-16 08:08:59.000000 lakers_python-0.3.0/crypto/lakers-crypto-rustcrypto/Cargo.toml
--rw-r--r--   0   671610   202045     5225 2024-02-02 13:05:06.000000 lakers_python-0.3.0/crypto/lakers-crypto-rustcrypto/src/lib.rs
--rw-r--r--   0   671610   202045      387 2024-02-16 09:54:33.000000 lakers_python-0.3.0/ead/lakers-ead-authz/Cargo.toml
--rw-r--r--   0   671610   202045      633 2024-03-07 10:47:35.000000 lakers_python-0.3.0/ead/lakers-ead-authz/cbindgen.toml
--rw-r--r--   0   671610   202045     7151 2024-04-05 13:20:00.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/authenticator.rs
--rw-r--r--   0   671610   202045     7458 2024-04-05 13:20:00.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/device.rs
--rw-r--r--   0   671610   202045     3522 2024-04-05 13:20:00.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/lib.rs
--rw-r--r--   0   671610   202045    13076 2024-04-05 13:20:00.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/server.rs
--rw-r--r--   0   671610   202045     7453 2024-04-05 13:20:00.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/shared.rs
--rw-r--r--   0   671610   202045     3766 2024-01-16 14:15:54.000000 lakers_python-0.3.0/ead/lakers-ead-authz/src/test_vectors.rs
--rw-r--r--   0   671610   202045      618 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lib/Cargo.toml
--rw-r--r--   0   671610   202045     6054 2024-04-05 13:20:00.000000 lakers_python-0.3.0/lib/README.md
--rw-r--r--   0   671610   202045    58361 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lib/src/edhoc.rs
--rw-r--r--   0   671610   202045    25819 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lib/src/lib.rs
--rw-r--r--   0   671610   202045     1276 2024-04-05 13:20:00.000000 lakers_python-0.3.0/crypto/Cargo.toml
--rw-r--r--   0   671610   202045      290 2023-05-09 08:42:52.000000 lakers_python-0.3.0/crypto/.cargo/config.toml
--rw-r--r--   0   671610   202045     3039 2024-04-05 13:20:00.000000 lakers_python-0.3.0/crypto/src/lib.rs
--rw-r--r--   0   671610   202045      574 2024-04-05 13:20:00.000000 lakers_python-0.3.0/shared/Cargo.toml
--rw-r--r--   0   671610   202045      832 2024-03-07 15:22:47.000000 lakers_python-0.3.0/shared/cbindgen.toml
--rw-r--r--   0   671610   202045     3081 2024-04-05 13:20:00.000000 lakers_python-0.3.0/shared/src/cred.rs
--rw-r--r--   0   671610   202045     2110 2024-02-02 13:05:06.000000 lakers_python-0.3.0/shared/src/crypto.rs
--rw-r--r--   0   671610   202045    32584 2024-05-13 12:19:21.000000 lakers_python-0.3.0/shared/src/lib.rs
--rw-r--r--   0   671610   202045     1511 2024-02-29 11:00:51.000000 lakers_python-0.3.0/shared/src/python_bindings.rs
--rw-r--r--   0   671610   202045      391 2024-01-16 08:08:59.000000 lakers_python-0.3.0/crypto/lakers-crypto-psa/Cargo.toml
--rw-r--r--   0   671610   202045    10617 2024-03-13 14:06:27.000000 lakers_python-0.3.0/crypto/lakers-crypto-psa/src/lib.rs
--rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 lakers_python-0.3.0/lakers-python/Cargo.toml
--rw-r--r--   0   671610   202045      764 2024-02-08 15:19:49.000000 lakers_python-0.3.0/lakers-python/README.md
--rw-r--r--   0   671610   202045     1398 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/ead_authz/authenticator.rs
--rw-r--r--   0   671610   202045     2139 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/ead_authz/device.rs
--rw-r--r--   0   671610   202045      107 2024-02-29 11:00:51.000000 lakers_python-0.3.0/lakers-python/src/ead_authz/mod.rs
--rw-r--r--   0   671610   202045     2419 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/ead_authz/server.rs
--rw-r--r--   0   671610   202045     6083 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/initiator.rs
--rw-r--r--   0   671610   202045     3046 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/lib.rs
--rw-r--r--   0   671610   202045     4915 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/src/responder.rs
--rw-r--r--   0   671610   202045     4496 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/test/test_ead_authz.py
--rw-r--r--   0   671610   202045     3152 2024-05-13 12:19:21.000000 lakers_python-0.3.0/lakers-python/test/test_lakers.py
--rw-r--r--   0   671610   202045        6 2024-02-08 15:19:49.000000 lakers_python-0.3.0/lakers-python/test_requirements.txt
--rw-r--r--   0   671610   202045    57821 2024-05-13 12:28:36.000000 lakers_python-0.3.0/Cargo.lock
--rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 lakers_python-0.3.0/Cargo.toml
--rw-r--r--   0        0        0      141 1970-01-01 00:00:00.000000 lakers_python-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 lakers_python-0.3.0/PKG-INFO
+-rw-r--r--   0     1001      127      384 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/Cargo.toml
+-rw-r--r--   0     1001      127     1580 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/build.rs
+-rw-r--r--   0     1001      127     2050 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/src/c/wrapper.h
+-rw-r--r--   0     1001      127    10187 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/src/lib.rs
+-rw-r--r--   0     1001      127      771 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile
+-rw-r--r--   0     1001      127     1217 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile.internal
+-rw-r--r--   0     1001      127     4213 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_defs.h
+-rw-r--r--   0     1001      127     4680 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_utils.c
+-rw-r--r--   0     1001      127    13789 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_data.h
+-rw-r--r--   0     1001      127     3989 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_defs.h
+-rw-r--r--   0     1001      127     6951 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ccsw_crys_rsa_shared_types.h
+-rw-r--r--   0     1001      127    18924 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm.h
+-rw-r--r--   0     1001      127     7180 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm_error.h
+-rw-r--r--   0     1001      127    12210 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha.h
+-rw-r--r--   0     1001      127     5299 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_error.h
+-rw-r--r--   0     1001      127     5336 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly.h
+-rw-r--r--   0     1001      127     4848 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly_error.h
+-rw-r--r--   0     1001      127    17291 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common.h
+-rw-r--r--   0     1001      127     5103 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common_error.h
+-rw-r--r--   0     1001      127    28262 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh.h
+-rw-r--r--   0     1001      127     8030 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_error.h
+-rw-r--r--   0     1001      127    12591 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_kg.h
+-rw-r--r--   0     1001      127    11841 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_edw_api.h
+-rw-r--r--   0     1001      127    13273 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_api.h
+-rw-r--r--   0     1001      127     6273 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_edw_error.h
+-rw-r--r--   0     1001      127    13454 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_build.h
+-rw-r--r--   0     1001      127     5126 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_dh.h
+-rw-r--r--   0     1001      127     3832 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_domain.h
+-rw-r--r--   0     1001      127     8772 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_ecdsa.h
+-rw-r--r--   0     1001      127    19639 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_error.h
+-rw-r--r--   0     1001      127     4757 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_kg.h
+-rw-r--r--   0     1001      127    19193 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_types.h
+-rw-r--r--   0     1001      127    12890 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_error.h
+-rw-r--r--   0     1001      127    13780 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash.h
+-rw-r--r--   0     1001      127     3376 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_defs.h
+-rw-r--r--   0     1001      127     5101 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_error.h
+-rw-r--r--   0     1001      127     6138 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf.h
+-rw-r--r--   0     1001      127     4247 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf_error.h
+-rw-r--r--   0     1001      127    11821 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac.h
+-rw-r--r--   0     1001      127     3374 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_defs.h
+-rw-r--r--   0     1001      127     5259 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_error.h
+-rw-r--r--   0     1001      127    10891 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf.h
+-rw-r--r--   0     1001      127     5154 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf_error.h
+-rw-r--r--   0     1001      127     7450 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_pka_defs_hw.h
+-rw-r--r--   0     1001      127     4998 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly.h
+-rw-r--r--   0     1001      127     4170 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly_error.h
+-rw-r--r--   0     1001      127    19714 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd.h
+-rw-r--r--   0     1001      127     8213 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd_error.h
+-rw-r--r--   0     1001      127     9721 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_build.h
+-rw-r--r--   0     1001      127    16219 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_error.h
+-rw-r--r--   0     1001      127     7582 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_kg.h
+-rw-r--r--   0     1001      127     7921 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_prim.h
+-rw-r--r--   0     1001      127    34649 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_schemes.h
+-rw-r--r--   0     1001      127    23132 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_types.h
+-rw-r--r--   0     1001      127    17872 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp.h
+-rw-r--r--   0     1001      127     4401 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp_error.h
+-rw-r--r--   0     1001      127     3641 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/dx_reg_base_host.h
+-rw-r--r--   0     1001      127     4914 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/sns_silib.h
+-rw-r--r--   0     1001      127    17381 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes.h
+-rw-r--r--   0     1001      127     4168 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_defs.h
+-rw-r--r--   0     1001      127     7180 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_error.h
+-rw-r--r--   0     1001      127     4233 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_bitops.h
+-rw-r--r--   0     1001      127     3536 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_abort.h
+-rw-r--r--   0     1001      127     3700 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_barrier.h
+-rw-r--r--   0     1001      127     8494 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_compiler.h
+-rw-r--r--   0     1001      127     9900 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma.h
+-rw-r--r--   0     1001      127     4089 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_defs.h
+-rw-r--r--   0     1001      127     3582 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_plat.h
+-rw-r--r--   0     1001      127     4187 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_error.h
+-rw-r--r--   0     1001      127     9241 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file.h
+-rw-r--r--   0     1001      127     5012 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file_plat.h
+-rw-r--r--   0     1001      127     4816 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_fips.h
+-rw-r--r--   0     1001      127     4021 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_init.h
+-rw-r--r--   0     1001      127     4605 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_list.h
+-rw-r--r--   0     1001      127     9188 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_log.h
+-rw-r--r--   0     1001      127     7156 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mem.h
+-rw-r--r--   0     1001      127     4487 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_memmap.h
+-rw-r--r--   0     1001      127     5729 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex.h
+-rw-r--r--   0     1001      127     3606 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex_plat.h
+-rw-r--r--   0     1001      127     5696 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf.h
+-rw-r--r--   0     1001      127     3287 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf_plat.h
+-rw-r--r--   0     1001      127     5074 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem.h
+-rw-r--r--   0     1001      127     5028 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem_plat.h
+-rw-r--r--   0     1001      127     3426 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_trng.h
+-rw-r--r--   0     1001      127     5532 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types.h
+-rw-r--r--   0     1001      127     3458 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types_plat.h
+-rw-r--r--   0     1001      127     3885 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pka_hw_plat_defs.h
+-rw-r--r--   0     1001      127     8745 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_regs.h
+-rw-r--r--   0     1001      127     3742 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_sram_map.h
+-rw-r--r--   0     1001      127     4544 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_defs.h
+-rw-r--r--   0     1001      127     5141 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_error.h
+-rw-r--r--   0     1001      127     5670 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation.h
+-rw-r--r--   0     1001      127     4277 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation_defs.h
+-rw-r--r--   0     1001      127   297096 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/libnrf_cc310_0.9.13.a
+-rw-r--r--   0     1001      127   296510 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/no-interrupts/libnrf_cc310_0.9.13.a
+-rw-r--r--   0     1001      127   297096 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/libnrf_cc310_0.9.13.a
+-rw-r--r--   0     1001      127   296510 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a
+-rw-r--r--   0     1001      127   296510 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib
+-rw-r--r--   0     1001      127   297096 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/nrf_cc310_0.9.13.lib
+-rw-r--r--   0     1001      127   295748 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/libnrf_cc310_0.9.13.a
+-rw-r--r--   0     1001      127   295162 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/no-interrupts/libnrf_cc310_0.9.13.a
+-rw-r--r--   0     1001      127   295748 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/libnrf_cc310_0.9.13.a
+-rw-r--r--   0     1001      127   295162 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a
+-rw-r--r--   0     1001      127   295162 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib
+-rw-r--r--   0     1001      127   295748 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/nrf_cc310_0.9.13.lib
+-rw-r--r--   0     1001      127     1501 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/license.txt
+-rw-r--r--   0     1001      127     1501 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/license.txt
+-rw-r--r--   0     1001      127      136 2024-05-17 14:16:50.000000 lakers_python-0.3.1/shared/README.md
+-rw-r--r--   0     1001      127      387 2024-05-17 14:16:50.000000 lakers_python-0.3.1/ead/lakers-ead-authz/Cargo.toml
+-rw-r--r--   0     1001      127      633 2024-05-17 14:16:50.000000 lakers_python-0.3.1/ead/lakers-ead-authz/cbindgen.toml
+-rw-r--r--   0     1001      127     7151 2024-05-17 14:16:50.000000 lakers_python-0.3.1/ead/lakers-ead-authz/src/authenticator.rs
+-rw-r--r--   0     1001      127     7458 2024-05-17 14:16:50.000000 lakers_python-0.3.1/ead/lakers-ead-authz/src/device.rs
+-rw-r--r--   0     1001      127     3522 2024-05-17 14:16:50.000000 lakers_python-0.3.1/ead/lakers-ead-authz/src/lib.rs
+-rw-r--r--   0     1001      127    13076 2024-05-17 14:16:50.000000 lakers_python-0.3.1/ead/lakers-ead-authz/src/server.rs
+-rw-r--r--   0     1001      127     7453 2024-05-17 14:16:50.000000 lakers_python-0.3.1/ead/lakers-ead-authz/src/shared.rs
+-rw-r--r--   0     1001      127     3766 2024-05-17 14:16:50.000000 lakers_python-0.3.1/ead/lakers-ead-authz/src/test_vectors.rs
+-rw-r--r--   0     1001      127      753 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-rustcrypto/Cargo.toml
+-rw-r--r--   0     1001      127     5225 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/lakers-crypto-rustcrypto/src/lib.rs
+-rw-r--r--   0     1001      127      618 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lib/Cargo.toml
+-rw-r--r--   0     1001      127     6054 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lib/README.md
+-rw-r--r--   0     1001      127    59732 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lib/src/edhoc.rs
+-rw-r--r--   0     1001      127    25819 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lib/src/lib.rs
+-rw-r--r--   0     1001      127     1276 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/Cargo.toml
+-rw-r--r--   0     1001      127      290 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/.cargo/config.toml
+-rw-r--r--   0     1001      127     3039 2024-05-17 14:16:50.000000 lakers_python-0.3.1/crypto/src/lib.rs
+-rw-r--r--   0     1001      127      626 2024-05-17 14:16:50.000000 lakers_python-0.3.1/shared/Cargo.toml
+-rw-r--r--   0     1001      127      832 2024-05-17 14:16:50.000000 lakers_python-0.3.1/shared/cbindgen.toml
+-rw-r--r--   0     1001      127     3131 2024-05-17 14:16:50.000000 lakers_python-0.3.1/shared/src/cred.rs
+-rw-r--r--   0     1001      127     2110 2024-05-17 14:16:50.000000 lakers_python-0.3.1/shared/src/crypto.rs
+-rw-r--r--   0     1001      127    33422 2024-05-17 14:16:50.000000 lakers_python-0.3.1/shared/src/lib.rs
+-rw-r--r--   0     1001      127     3818 2024-05-17 14:16:50.000000 lakers_python-0.3.1/shared/src/python_bindings.rs
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 lakers_python-0.3.1/lakers-python/Cargo.toml
+-rw-r--r--   0     1001      127     1015 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/README.md
+-rw-r--r--   0     1001      127     2091 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/examples/coapclient.rs.rust
+-rw-r--r--   0     1001      127       38 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/examples/lakers-c-native/.gitignore
+-rw-r--r--   0     1001      127      633 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/examples/lakers-c-native/Makefile
+-rw-r--r--   0     1001      127      813 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/examples/lakers-c-native/README.md
+-rw-r--r--   0     1001      127     8838 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/examples/lakers-c-native/main.c
+-rw-r--r--   0     1001      127        4 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/examples/lakers-c-riot/.gitignore
+-rw-r--r--   0     1001      127      945 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/examples/lakers-c-riot/Makefile
+-rw-r--r--   0     1001      127      593 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/examples/lakers-c-riot/README.md
+-rw-r--r--   0     1001      127     4168 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/examples/lakers-c-riot/main.c
+-rw-r--r--   0     1001      127    29797 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/examples/traces-zeroconf.ipynb
+-rw-r--r--   0     1001      127     1398 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/src/ead_authz/authenticator.rs
+-rw-r--r--   0     1001      127     2139 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/src/ead_authz/device.rs
+-rw-r--r--   0     1001      127      107 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/src/ead_authz/mod.rs
+-rw-r--r--   0     1001      127     2419 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/src/ead_authz/server.rs
+-rw-r--r--   0     1001      127     5960 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/src/initiator.rs
+-rw-r--r--   0     1001      127     3771 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/src/lib.rs
+-rw-r--r--   0     1001      127     4788 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/src/responder.rs
+-rw-r--r--   0     1001      127     4496 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/test/test_ead_authz.py
+-rw-r--r--   0     1001      127     4146 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/test/test_lakers.py
+-rw-r--r--   0     1001      127        6 2024-05-17 14:16:50.000000 lakers_python-0.3.1/lakers-python/test_requirements.txt
+-rw-r--r--   0     1001      127    58975 2024-05-17 14:17:13.000000 lakers_python-0.3.1/Cargo.lock
+-rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 lakers_python-0.3.1/Cargo.toml
+-rw-r--r--   0        0        0      160 1970-01-01 00:00:00.000000 lakers_python-0.3.1/pyproject.toml
+-rw-r--r--   0     1001      127     2091 2024-05-17 14:16:50.000000 lakers_python-0.3.1/examples/coapclient.rs.rust
+-rw-r--r--   0     1001      127    29797 2024-05-17 14:16:50.000000 lakers_python-0.3.1/examples/traces-zeroconf.ipynb
+-rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 lakers_python-0.3.1/PKG-INFO
```

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/build.rs` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/build.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/src/c/wrapper.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/src/c/wrapper.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/src/lib.rs` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile.internal` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/Doxyfile.internal`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_defs.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_utils.c` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_plat_utils.c`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_data.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_data.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_defs.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/common/integration_test_ssi_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ccsw_crys_rsa_shared_types.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ccsw_crys_rsa_shared_types.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_aesccm_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_chacha_poly_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_common_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_kg.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_dh_kg.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_edw_api.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_edw_api.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_api.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_api.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_edw_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ec_mont_edw_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_build.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_build.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_dh.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_dh.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_domain.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_domain.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_ecdsa.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_ecdsa.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_kg.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_kg.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_types.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_ecpki_types.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_defs.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hash_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hkdf_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_defs.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_hmac_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_kdf_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_pka_defs_hw.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_pka_defs_hw.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_poly_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rnd_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_build.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_build.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_kg.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_kg.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_prim.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_prim.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_schemes.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_schemes.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_types.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_rsa_types.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/crys_srp_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/dx_reg_base_host.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/dx_reg_base_host.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/sns_silib.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/sns_silib.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_defs.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_aes_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_bitops.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_bitops.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_abort.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_abort.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_barrier.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_barrier.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_compiler.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_compiler.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_defs.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_plat.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_dma_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file_plat.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_file_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_fips.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_fips.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_init.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_init.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_list.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_list.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_log.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_log.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mem.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mem.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_memmap.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_memmap.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex_plat.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_mutex_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf_plat.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_perf_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem_plat.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_sem_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_trng.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_trng.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types_plat.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pal_types_plat.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pka_hw_plat_defs.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_pka_hw_plat_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_regs.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_regs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_sram_map.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_sram_map.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_defs.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_error.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_error.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation_defs.h` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/include/ssi_util_key_derivation_defs.h`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/no-interrupts/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/no-interrupts/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/nrf_cc310_0.9.13.lib` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/hard-float/short-wchar/nrf_cc310_0.9.13.lib`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/no-interrupts/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/no-interrupts/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/libnrf_cc310_0.9.13.a`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/no-interrupts/nrf_cc310_0.9.13.lib`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/nrf_cc310_0.9.13.lib` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/cortex-m4/soft-float/short-wchar/nrf_cc310_0.9.13.lib`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/license.txt` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/lib/license.txt`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/license.txt` & `lakers_python-0.3.1/crypto/lakers-crypto-cryptocell310-sys/vendor/nrf_cc310/license.txt`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-rustcrypto/Cargo.toml` & `lakers_python-0.3.1/crypto/lakers-crypto-rustcrypto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/lakers-crypto-rustcrypto/src/lib.rs` & `lakers_python-0.3.1/crypto/lakers-crypto-rustcrypto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/ead/lakers-ead-authz/cbindgen.toml` & `lakers_python-0.3.1/ead/lakers-ead-authz/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/ead/lakers-ead-authz/src/authenticator.rs` & `lakers_python-0.3.1/ead/lakers-ead-authz/src/authenticator.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/ead/lakers-ead-authz/src/device.rs` & `lakers_python-0.3.1/ead/lakers-ead-authz/src/device.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/ead/lakers-ead-authz/src/lib.rs` & `lakers_python-0.3.1/ead/lakers-ead-authz/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/ead/lakers-ead-authz/src/server.rs` & `lakers_python-0.3.1/ead/lakers-ead-authz/src/server.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/ead/lakers-ead-authz/src/shared.rs` & `lakers_python-0.3.1/ead/lakers-ead-authz/src/shared.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/ead/lakers-ead-authz/src/test_vectors.rs` & `lakers_python-0.3.1/ead/lakers-ead-authz/src/test_vectors.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/lib/Cargo.toml` & `lakers_python-0.3.1/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/lib/README.md` & `lakers_python-0.3.1/lib/README.md`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/lib/src/edhoc.rs` & `lakers_python-0.3.1/lib/src/edhoc.rs`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,25 @@
                     public_key: Default::default(),
                     kid,
                 },
                 IdCred::FullCredential(cred) => {
                     let Ok(buffer) = EdhocMessageBuffer::new_from_slice(cred) else {
                         return Err(EDHOCError::ParsingError);
                     };
-                    CredentialRPK::new(buffer)?
+                    if let Ok(parsed_rpk) = CredentialRPK::new(buffer) {
+                        parsed_rpk
+                    } else {
+                        // This is incomplete, and the application will need to fill in the gaps --
+                        // just as in the CompactKid case the CredentialRPK is also incomplete.
+                        CredentialRPK {
+                            value: buffer,
+                            public_key: Default::default(),
+                            kid: Default::default(),
+                        }
+                    }
                 }
             };
 
             Ok((
                 ProcessingM3 {
                     mac_3,
                     y: state.y,
@@ -411,16 +421,19 @@
         &state.prk_4e3m,
         &state.th_3,
         &cred_i.get_id_cred(),
         cred_i.value.as_slice(),
         ead_3,
     );
 
-    assert!(matches!(cred_transfer, CredentialTransfer::ByReference)); // TODO: handle ByValue case as well
-    let plaintext_3 = encode_plaintext_3(&cred_i.get_id_cred(), &mac_3, &ead_3)?;
+    let id_cred_i = match cred_transfer {
+        CredentialTransfer::ByValue => IdCred::FullCredential(cred_i.value.as_slice()),
+        CredentialTransfer::ByReference => IdCred::CompactKid(cred_i.kid),
+    };
+    let plaintext_3 = encode_plaintext_3(&id_cred_i, &mac_3, &ead_3)?;
     let message_3 = encrypt_message_3(crypto, &state.prk_3e2m, &state.th_3, &plaintext_3);
 
     let th_4 = compute_th_4(crypto, &state.th_3, &plaintext_3, cred_i.value.as_slice());
 
     let mut th_4_buf: BytesMaxContextBuffer = [0x00; MAX_KDF_CONTEXT_LEN];
     th_4_buf[..th_4.len()].copy_from_slice(&th_4[..]);
 
@@ -634,25 +647,26 @@
 ) -> BytesMaxBuffer {
     let (info, info_len) = encode_info(label, context, context_len, length);
 
     crypto.hkdf_expand(prk, &info, info_len, length)
 }
 
 fn encode_plaintext_3(
-    id_cred_i: &BytesIdCred,
+    id_cred_i: &IdCred,
     mac_3: &BytesMac3,
     ead_3: &Option<EADItem>,
 ) -> Result<BufferPlaintext3, EDHOCError> {
     let mut plaintext_3: BufferPlaintext3 = BufferPlaintext3::new();
 
     // plaintext: P = ( ? PAD, ID_CRED_I / bstr / int, Signature_or_MAC_3, ? EAD_3 )
-    plaintext_3.content[0] = id_cred_i[id_cred_i.len() - 1]; // hack: take the last byte of ID_CRED_I as KID
-    plaintext_3.content[1] = CBOR_MAJOR_BYTE_STRING | MAC_LENGTH_3 as u8;
-    plaintext_3.content[2..2 + mac_3.len()].copy_from_slice(&mac_3[..]);
-    plaintext_3.len = 2 + mac_3.len();
+    id_cred_i.write_to_message(&mut plaintext_3)?;
+    let offset_cred = plaintext_3.len;
+    plaintext_3.content[offset_cred] = CBOR_MAJOR_BYTE_STRING | MAC_LENGTH_3 as u8;
+    plaintext_3.content[offset_cred + 1..][..mac_3.len()].copy_from_slice(&mac_3[..]);
+    plaintext_3.len = offset_cred + 1 + mac_3.len();
 
     if let Some(ead_3) = ead_3 {
         match encode_ead_item(ead_3) {
             Ok(ead_3) => plaintext_3
                 .extend_from_slice(ead_3.as_slice())
                 .and(Ok(plaintext_3))
                 .or(Err(EDHOCError::EadTooLongError)),
@@ -719,40 +733,67 @@
 fn encrypt_message_3(
     crypto: &mut impl CryptoTrait,
     prk_3e2m: &BytesHashLen,
     th_3: &BytesHashLen,
     plaintext_3: &BufferPlaintext3,
 ) -> BufferMessage3 {
     let mut output: BufferMessage3 = BufferMessage3::new();
-    output.len = 1 + plaintext_3.len + AES_CCM_TAG_LEN;
-    output.content[0] = CBOR_MAJOR_BYTE_STRING | (plaintext_3.len + AES_CCM_TAG_LEN) as u8; // FIXME if plaintext_3.len + AES_CCM_TAG_LEN > 23, then should use CBOR_BYTE_STRING
+    let bytestring_length = plaintext_3.len + AES_CCM_TAG_LEN;
+    let prefix_length;
+    // FIXME: Reuse CBOR encoder
+    if bytestring_length < 24 {
+        output.content[0] = CBOR_MAJOR_BYTE_STRING | (bytestring_length) as u8;
+        prefix_length = 1;
+    } else {
+        // FIXME: Assumes we don't exceed 256 bytes which is the current buffer size
+        output.content[0] = CBOR_MAJOR_BYTE_STRING | 24;
+        output.content[1] = bytestring_length as _;
+        prefix_length = 2;
+    };
+    output.len = prefix_length + bytestring_length;
+    // FIXME: Make the function fallible, especially with the prospect of algorithm agility
+    assert!(
+        output.len <= MAX_MESSAGE_SIZE_LEN,
+        "Tried to encode a message that is too large."
+    );
 
     let enc_structure = encode_enc_structure(th_3);
 
     let (k_3, iv_3) = compute_k_3_iv_3(crypto, prk_3e2m, th_3);
 
     let ciphertext_3 = crypto.aes_ccm_encrypt_tag_8(&k_3, &iv_3, &enc_structure[..], plaintext_3);
 
-    output.content[1..output.len].copy_from_slice(ciphertext_3.as_slice());
+    output.content[prefix_length..][..ciphertext_3.len].copy_from_slice(ciphertext_3.as_slice());
 
     output
 }
 
 fn decrypt_message_3(
     crypto: &mut impl CryptoTrait,
     prk_3e2m: &BytesHashLen,
     th_3: &BytesHashLen,
     message_3: &BufferMessage3,
 ) -> Result<BufferPlaintext3, EDHOCError> {
     // decode message_3
-    let len = (message_3.content[0usize] ^ CBOR_MAJOR_BYTE_STRING) as usize;
+    let bytestring_length: usize;
+    let prefix_length;
+    // FIXME: Reuse CBOR decoder
+    if (0..=23).contains(&(message_3.content[0] ^ CBOR_MAJOR_BYTE_STRING)) {
+        bytestring_length = (message_3.content[0] ^ CBOR_MAJOR_BYTE_STRING).into();
+        prefix_length = 1;
+    } else {
+        // FIXME: Assumes we don't exceed 256 bytes which is the current buffer size
+        bytestring_length = message_3.content[1].into();
+        prefix_length = 2;
+    }
 
     let mut ciphertext_3: BufferCiphertext3 = BufferCiphertext3::new();
-    ciphertext_3.len = len;
-    ciphertext_3.content[..len].copy_from_slice(&message_3.content[1..1 + len]);
+    ciphertext_3.len = bytestring_length;
+    ciphertext_3.content[..bytestring_length]
+        .copy_from_slice(&message_3.content[prefix_length..][..bytestring_length]);
 
     let (k_3, iv_3) = compute_k_3_iv_3(crypto, prk_3e2m, th_3);
 
     let enc_structure = encode_enc_structure(th_3);
 
     crypto.aes_ccm_decrypt_tag_8(&k_3, &iv_3, &enc_structure, &ciphertext_3)
 }
@@ -849,28 +890,20 @@
     c_r: ConnId,
     id_cred_r: &IdCred,
     mac_2: &BytesMac2,
     ead_2: &Option<EADItem>,
 ) -> Result<BufferPlaintext2, EDHOCError> {
     let mut plaintext_2: BufferPlaintext2 = BufferPlaintext2::new();
     let c_r = c_r.as_slice();
-    plaintext_2.content[..c_r.len()].copy_from_slice(c_r);
 
-    let offset_cred = match id_cred_r {
-        IdCred::CompactKid(kid) => {
-            plaintext_2.content[c_r.len()] = *kid;
-            c_r.len() + 1
-        }
-        IdCred::FullCredential(cred) => {
-            plaintext_2.content[c_r.len()] = CBOR_BYTE_STRING;
-            plaintext_2.content[c_r.len() + 1] = cred.len() as u8;
-            plaintext_2.content[c_r.len() + 2..][..cred.len()].copy_from_slice(cred);
-            c_r.len() + 2 + cred.len()
-        }
-    };
+    plaintext_2
+        .extend_from_slice(c_r)
+        .or(Err(EDHOCError::EncodingError))?;
+    id_cred_r.write_to_message(&mut plaintext_2)?;
+    let offset_cred = plaintext_2.len;
 
     plaintext_2.content[offset_cred] = CBOR_MAJOR_BYTE_STRING | MAC_LENGTH_2 as u8;
     plaintext_2.content[1 + offset_cred..1 + offset_cred + mac_2.len()].copy_from_slice(&mac_2[..]);
     plaintext_2.len = 1 + offset_cred + mac_2.len();
 
     if let Some(ead_2) = ead_2 {
         match encode_ead_item(ead_2) {
@@ -1458,15 +1491,17 @@
         let prk_2e = compute_prk_2e(&mut default_crypto(), &X_TV, &G_Y_TV, &TH_2_TV);
         assert_eq!(prk_2e, PRK_2E_TV);
     }
 
     #[test]
     fn test_encode_plaintext_3() {
         let plaintext_3_tv = BufferPlaintext3::from_hex(PLAINTEXT_3_TV);
-        let plaintext_3 = encode_plaintext_3(&ID_CRED_I_TV, &MAC_3_TV, &None::<EADItem>).unwrap();
+        let kid_tv = ID_CRED_I_TV[ID_CRED_I_TV.len() - 1];
+        let plaintext_3 =
+            encode_plaintext_3(&IdCred::CompactKid(kid_tv), &MAC_3_TV, &None::<EADItem>).unwrap();
         assert_eq!(plaintext_3, plaintext_3_tv);
     }
 
     #[test]
     fn test_decode_plaintext_3() {
         let plaintext_3_tv = BufferPlaintext3::from_hex(PLAINTEXT_3_TV);
         let kid_tv = ID_CRED_I_TV[ID_CRED_I_TV.len() - 1];
```

### Comparing `lakers_python-0.3.0/lib/src/lib.rs` & `lakers_python-0.3.1/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/Cargo.toml` & `lakers_python-0.3.1/crypto/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/crypto/src/lib.rs` & `lakers_python-0.3.1/crypto/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/shared/Cargo.toml` & `lakers_python-0.3.1/shared/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # It's implied, but still better for consistency to have it explicit.
 readme.workspace = true
 keywords.workspace = true
 categories.workspace = true
 
 [dependencies]
 pyo3 = { version = "0.20.2", features = ["extension-module"], optional = true }
+hex = { version = "0.4.3", optional = true }
 
 [dev-dependencies]
 hexlit = "0.5.3"
 
 [features]
 default = [  ]
-python-bindings = ["pyo3"]
+python-bindings = ["pyo3", "hex"]
```

### Comparing `lakers_python-0.3.0/shared/cbindgen.toml` & `lakers_python-0.3.1/shared/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/shared/src/cred.rs` & `lakers_python-0.3.1/shared/src/cred.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use super::*;
 
 #[derive(Clone, Copy, Debug)]
+#[cfg_attr(feature = "python-bindings", pyclass)]
 #[repr(C)]
 pub struct CredentialRPK {
     pub value: EdhocMessageBuffer,
     pub public_key: BytesP256ElemLen, // could be a reference, but safe Rust doesn't allow self-referencing structs
     pub kid: u8,
 }
```

### Comparing `lakers_python-0.3.0/shared/src/crypto.rs` & `lakers_python-0.3.1/shared/src/crypto.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/shared/src/lib.rs` & `lakers_python-0.3.1/shared/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,16 @@
     /// error: When the application sets the expected credential, that process should be informed
     /// by the known details.
     UnexpectedCredential,
     MacVerificationFailed,
     UnsupportedMethod,
     UnsupportedCipherSuite,
     ParsingError,
+    EncodingError,
+    CredentialTooLongError,
     EadLabelTooLongError,
     EadTooLongError,
     /// An EAD was received that was either not known (and critical), or not understood, or
     /// otherwise erroneous.
     EADUnprocessable,
     /// The credential or EADs could be processed (possibly by a third party), but the decision
     /// based on that was to not to continue the EDHOC session.
@@ -224,14 +226,16 @@
         use EDHOCError::*;
         match self {
             UnexpectedCredential => ErrCode::UNSPECIFIED,
             MacVerificationFailed => ErrCode::UNSPECIFIED,
             UnsupportedMethod => ErrCode::UNSPECIFIED,
             UnsupportedCipherSuite => ErrCode::WRONG_SELECTED_CIPHER_SUITE,
             ParsingError => ErrCode::UNSPECIFIED,
+            EncodingError => ErrCode::UNSPECIFIED,
+            CredentialTooLongError => ErrCode::UNSPECIFIED,
             EadLabelTooLongError => ErrCode::UNSPECIFIED,
             EadTooLongError => ErrCode::UNSPECIFIED,
             EADUnprocessable => ErrCode::UNSPECIFIED,
             AccessDenied => ErrCode::ACCESS_DENIED,
         }
     }
 }
@@ -491,14 +495,31 @@
 // FIXME: homogenize the two structs below (likey keep only the owned version)
 #[derive(Debug, Clone, Copy)]
 pub enum IdCred<'a> {
     CompactKid(u8),
     FullCredential(&'a [u8]),
 }
 
+impl<'a> IdCred<'a> {
+    pub fn write_to_message(&self, message: &mut EdhocMessageBuffer) -> Result<(), EDHOCError> {
+        match self {
+            IdCred::CompactKid(kid) => message.extend_from_slice(&[*kid]),
+            IdCred::FullCredential(cred) => {
+                let len =
+                    u8::try_from(cred.len()).map_err(|_| EDHOCError::CredentialTooLongError)?;
+                message
+                    .extend_from_slice(&[CBOR_BYTE_STRING, len])
+                    .map_err(|_| EDHOCError::CredentialTooLongError)?;
+                message.extend_from_slice(cred)
+            }
+        }
+        .map_err(|_| EDHOCError::CredentialTooLongError)
+    }
+}
+
 mod helpers {
     use super::*;
 
     pub fn encode_info(
         label: u8,
         context: &BytesMaxContextBuffer,
         context_len: usize,
```

### Comparing `lakers_python-0.3.0/lakers-python/Cargo.toml` & `lakers_python-0.3.1/lakers-python/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "lakers-python" # this will be the name of the package on pypi
 edition = "2021"
-version ="0.3.0"
+version ="0.3.1"
 repository.workspace = true
 license.workspace = true
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 pyo3 = { version = "0.20.2", features = ["extension-module"] }
```

### Comparing `lakers_python-0.3.0/lakers-python/src/ead_authz/authenticator.rs` & `lakers_python-0.3.1/lakers-python/src/ead_authz/authenticator.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/lakers-python/src/ead_authz/device.rs` & `lakers_python-0.3.1/lakers-python/src/ead_authz/device.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/lakers-python/src/ead_authz/server.rs` & `lakers_python-0.3.1/lakers-python/src/ead_authz/server.rs`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/lakers-python/src/initiator.rs` & `lakers_python-0.3.1/lakers-python/src/responder.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,138 +1,118 @@
 use lakers::*;
 use lakers_crypto::{default_crypto, CryptoTrait};
 use pyo3::{prelude::*, types::PyBytes};
 
-#[pyclass(name = "EdhocInitiator")]
-pub struct PyEdhocInitiator {
-    cred_i: Option<CredentialRPK>,
-    start: InitiatorStart,
-    wait_m2: WaitM2,
-    processing_m2: ProcessingM2,
-    processed_m2: ProcessedM2,
+#[pyclass(name = "EdhocResponder")]
+pub struct PyEdhocResponder {
+    r: Vec<u8>,
+    cred_r: CredentialRPK,
+    start: ResponderStart,
+    processing_m1: ProcessingM1,
+    wait_m3: WaitM3,
+    processing_m3: ProcessingM3,
     completed: Completed,
 }
 
 #[pymethods]
-impl PyEdhocInitiator {
+impl PyEdhocResponder {
     #[new]
-    fn new() -> Self {
-        // we only support a single cipher suite which is already CBOR-encoded
-        let mut suites_i: BytesSuites = [0x0; SUITES_LEN];
-        let suites_i_len = EDHOC_SUPPORTED_SUITES.len();
-        suites_i[0..suites_i_len].copy_from_slice(&EDHOC_SUPPORTED_SUITES[..]);
-        let (x, g_x) = default_crypto().p256_generate_key_pair();
-
-        Self {
-            cred_i: None,
-            start: InitiatorStart {
-                x,
-                g_x,
-                suites_i,
-                suites_i_len,
-            },
-            wait_m2: WaitM2::default(),
-            processing_m2: ProcessingM2::default(),
-            processed_m2: ProcessedM2::default(),
+    fn new(r: Vec<u8>, cred_r: super::AutoCredentialRPK) -> PyResult<Self> {
+        let (y, g_y) = default_crypto().p256_generate_key_pair();
+
+        let cred_r = cred_r.to_credential()?;
+
+        Ok(Self {
+            r,
+            cred_r,
+            start: ResponderStart { y, g_y },
+            processing_m1: ProcessingM1::default(),
+            wait_m3: WaitM3::default(),
+            processing_m3: ProcessingM3::default(),
             completed: Completed::default(),
-        }
+        })
     }
 
-    fn prepare_message_1<'a>(
+    fn process_message_1<'a>(
         &mut self,
         py: Python<'a>,
-        c_i: Option<Vec<u8>>,
-        ead_1: Option<EADItem>,
+        message_1: Vec<u8>,
+    ) -> PyResult<(&'a PyBytes, Option<EADItem>)> {
+        let message_1 = EdhocMessageBuffer::new_from_slice(message_1.as_slice())?;
+        let (state, c_i, ead_1) =
+            r_process_message_1(&self.start, &mut default_crypto(), &message_1)?;
+        self.processing_m1 = state;
+        let c_i = PyBytes::new(py, c_i.as_slice());
+
+        Ok((c_i, ead_1))
+    }
+
+    fn prepare_message_2<'a>(
+        &mut self,
+        py: Python<'a>,
+        cred_transfer: CredentialTransfer,
+        c_r: Option<Vec<u8>>,
+        ead_2: Option<EADItem>,
     ) -> PyResult<&'a PyBytes> {
-        let c_i = match c_i {
-            Some(c_i) => ConnId::from_slice(c_i.as_slice()).ok_or(
+        let c_r = match c_r {
+            Some(c_r) => ConnId::from_slice(c_r.as_slice()).ok_or(
                 pyo3::exceptions::PyValueError::new_err("Connection identifier out of range"),
             )?,
             None => generate_connection_identifier_cbor(&mut default_crypto()),
         };
+        let mut r = BytesP256ElemLen::default();
+        r.copy_from_slice(self.r.as_slice());
 
-        match i_prepare_message_1(&self.start, &mut default_crypto(), c_i, &ead_1) {
-            Ok((state, message_1)) => {
-                self.wait_m2 = state;
-                Ok(PyBytes::new(py, message_1.as_slice()))
+        match r_prepare_message_2(
+            &self.processing_m1,
+            &mut default_crypto(),
+            self.cred_r,
+            &r,
+            c_r,
+            cred_transfer,
+            &ead_2,
+        ) {
+            Ok((state, message_2)) => {
+                self.wait_m3 = state;
+                Ok(PyBytes::new(py, message_2.as_slice()))
             }
             Err(error) => Err(error.into()),
         }
     }
 
-    pub fn parse_message_2<'a>(
+    pub fn parse_message_3<'a>(
         &mut self,
         py: Python<'a>,
-        message_2: Vec<u8>,
-    ) -> PyResult<(&'a PyBytes, &'a PyBytes, Option<EADItem>)> {
-        let message_2 = EdhocMessageBuffer::new_from_slice(message_2.as_slice())?;
-
-        match i_parse_message_2(&self.wait_m2, &mut default_crypto(), &message_2) {
-            Ok((state, c_r, id_cred_r, ead_2)) => {
-                self.processing_m2 = state;
-                let id_cred_r = if id_cred_r.reference_only() {
-                    PyBytes::new(py, &[id_cred_r.kid])
+        message_3: Vec<u8>,
+    ) -> PyResult<(&'a PyBytes, Option<EADItem>)> {
+        let message_3 = EdhocMessageBuffer::new_from_slice(message_3.as_slice())?;
+        match r_parse_message_3(&mut self.wait_m3, &mut default_crypto(), &message_3) {
+            Ok((state, id_cred_i, ead_3)) => {
+                self.processing_m3 = state;
+                let id_cred_i = if id_cred_i.reference_only() {
+                    PyBytes::new(py, &[id_cred_i.kid])
                 } else {
-                    PyBytes::new(py, id_cred_r.value.as_slice())
+                    PyBytes::new(py, id_cred_i.value.as_slice())
                 };
-                let c_r = PyBytes::new(py, c_r.as_slice());
-                Ok((c_r, id_cred_r, ead_2))
-            }
-            Err(error) => Err(error.into()),
-        }
-    }
-
-    pub fn verify_message_2(
-        &mut self,
-        i: Vec<u8>,
-        cred_i: Vec<u8>,
-        valid_cred_r: Vec<u8>,
-    ) -> PyResult<()> {
-        let cred_i =
-            CredentialRPK::new(EdhocMessageBuffer::new_from_slice(&cred_i.as_slice()).unwrap())?;
-        let valid_cred_r = CredentialRPK::new(
-            EdhocMessageBuffer::new_from_slice(&valid_cred_r.as_slice()).unwrap(),
-        )?;
-
-        match i_verify_message_2(
-            &self.processing_m2,
-            &mut default_crypto(),
-            valid_cred_r,
-            i.as_slice()
-                .try_into()
-                .expect("Wrong length of initiator private key"),
-        ) {
-            Ok(state) => {
-                self.processed_m2 = state;
-                self.cred_i = Some(cred_i);
-                Ok(())
+                Ok((id_cred_i, ead_3))
             }
             Err(error) => Err(error.into()),
         }
     }
 
-    pub fn prepare_message_3<'a>(
+    pub fn verify_message_3<'a>(
         &mut self,
         py: Python<'a>,
-        cred_transfer: CredentialTransfer,
-        ead_3: Option<EADItem>,
-    ) -> PyResult<(&'a PyBytes, &'a PyBytes)> {
-        match i_prepare_message_3(
-            &mut self.processed_m2,
-            &mut default_crypto(),
-            self.cred_i.unwrap(),
-            cred_transfer,
-            &ead_3,
-        ) {
-            Ok((state, message_3, prk_out)) => {
+        valid_cred_i: super::AutoCredentialRPK,
+    ) -> PyResult<&'a PyBytes> {
+        let valid_cred_i = valid_cred_i.to_credential()?;
+        match r_verify_message_3(&mut self.processing_m3, &mut default_crypto(), valid_cred_i) {
+            Ok((state, prk_out)) => {
                 self.completed = state;
-                Ok((
-                    PyBytes::new(py, message_3.as_slice()),
-                    PyBytes::new(py, prk_out.as_slice()),
-                ))
+                Ok(PyBytes::new(py, prk_out.as_slice()))
             }
             Err(error) => Err(error.into()),
         }
     }
 
     pub fn edhoc_exporter<'a>(
         &mut self,
@@ -167,27 +147,8 @@
             &mut self.completed,
             &mut default_crypto(),
             &context_buf,
             context.len(),
         );
         Ok(PyBytes::new(py, &res[..SHA256_DIGEST_LEN]))
     }
-
-    pub fn get_h_message_1<'a>(&self, py: Python<'a>) -> PyResult<&'a PyBytes> {
-        Ok(PyBytes::new(py, &self.wait_m2.h_message_1[..]))
-    }
-
-    pub fn compute_ephemeral_secret<'a>(
-        &self,
-        py: Python<'a>,
-        g_a: Vec<u8>,
-    ) -> PyResult<&'a PyBytes> {
-        let mut g_a_arr = BytesP256ElemLen::default();
-        g_a_arr.copy_from_slice(&g_a[..]);
-        let secret = default_crypto().p256_ecdh(&self.start.x, &g_a_arr);
-        Ok(PyBytes::new(py, &secret[..]))
-    }
-
-    pub fn selected_cipher_suite(&self) -> PyResult<u8> {
-        Ok(self.start.suites_i[self.start.suites_i_len - 1])
-    }
 }
```

### Comparing `lakers_python-0.3.0/lakers-python/src/lib.rs` & `lakers_python-0.3.1/lakers-python/src/lib.rs`

 * *Files 27% similar despite different names*

```diff
@@ -16,23 +16,18 @@
 
 #[pyfunction(name = "credential_check_or_fetch")]
 // FIXME: using inverted parameters from rust version (credential_check_or_fetch)
 // since, in Python, by convention, parameters that can be None come later
 pub fn py_credential_check_or_fetch<'a>(
     py: Python<'a>,
     id_cred_received: Vec<u8>,
-    cred_expected: Option<Vec<u8>>,
+    cred_expected: Option<AutoCredentialRPK>,
 ) -> PyResult<&'a PyBytes> {
-    let cred_expected = if let Some(cred_expected) = cred_expected {
-        Some(CredentialRPK::new(
-            EdhocMessageBuffer::new_from_slice(cred_expected.as_slice()).unwrap(),
-        )?)
-    } else {
-        None
-    };
+    let cred_expected = cred_expected.map(|c| c.to_credential()).transpose()?;
+
     let valid_cred = if id_cred_received.len() == 1 {
         credential_check_or_fetch(
             cred_expected,
             CredentialRPK {
                 kid: id_cred_received[0],
                 value: Default::default(),
                 public_key: Default::default(),
@@ -55,25 +50,48 @@
     let (x, g_x) = default_crypto().p256_generate_key_pair();
     Ok((
         PyBytes::new(py, x.as_slice()),
         PyBytes::new(py, g_x.as_slice()),
     ))
 }
 
+/// Helper for PyO3 converted functions that behave like passing an argument through a
+/// `CredentialRPK` constructor; use this in an argument and then call [self.to_credential()].
+/// The resulting function will accept both a bytes-ish object (and pass it through
+/// [CredentialRPK::new()] or a preexisting [CredentialRPK].
+#[derive(FromPyObject)]
+enum AutoCredentialRPK {
+    #[pyo3(transparent, annotation = "bytes")]
+    Parse(Vec<u8>),
+    #[pyo3(transparent, annotation = "CredentialRPK")]
+    Existing(lakers_shared::CredentialRPK),
+}
+
+impl AutoCredentialRPK {
+    fn to_credential(self) -> PyResult<CredentialRPK> {
+        use AutoCredentialRPK::*;
+        Ok(match self {
+            Existing(e) => e,
+            Parse(v) => CredentialRPK::new(EdhocMessageBuffer::new_from_slice(&v)?)?,
+        })
+    }
+}
+
 // this name must match `lib.name` in `Cargo.toml`
 #[pymodule]
 #[pyo3(name = "lakers")]
 fn lakers_python(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(p256_generate_key_pair, m)?)?;
     m.add_function(wrap_pyfunction!(py_credential_check_or_fetch, m)?)?;
     // edhoc items
     m.add_class::<initiator::PyEdhocInitiator>()?;
     m.add_class::<responder::PyEdhocResponder>()?;
     m.add_class::<lakers::CredentialTransfer>()?;
     m.add_class::<lakers::EADItem>()?;
+    m.add_class::<lakers::CredentialRPK>()?;
     // ead-authz items
     m.add_class::<ead_authz::PyAuthzDevice>()?;
     m.add_class::<ead_authz::PyAuthzAutenticator>()?;
     m.add_class::<ead_authz::PyAuthzEnrollmentServer>()?;
     m.add_class::<ead_authz::PyAuthzServerUserAcl>()?;
 
     let submodule = PyModule::new(_py, "consts")?;
```

### Comparing `lakers_python-0.3.0/lakers-python/test/test_ead_authz.py` & `lakers_python-0.3.1/lakers-python/test/test_ead_authz.py`

 * *Files identical despite different names*

### Comparing `lakers_python-0.3.0/lakers-python/test/test_lakers.py` & `lakers_python-0.3.1/lakers-python/test/test_lakers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import lakers
+import cbor2
 import pytest
 
-# values from RFC9529
-CRED_I = bytes.fromhex("A2027734322D35302D33312D46462D45462D33372D33322D333908A101A5010202412B2001215820AC75E9ECE3E50BFC8ED60399889522405C47BF16DF96660A41298CB4307F7EB62258206E5DE611388A4B8A8211334AC7D37ECB52A387D257E6DB3C2A93DF21FF3AFFC8")
+# values from RFC9529, but CRED_I shortened so that passing by value is possible in a 256 byte message
+CRED_I = bytes.fromhex("A202617808A101A5010202412B2001215820AC75E9ECE3E50BFC8ED60399889522405C47BF16DF96660A41298CB4307F7EB62258206E5DE611388A4B8A8211334AC7D37ECB52A387D257E6DB3C2A93DF21FF3AFFC8")
 I = bytes.fromhex("fb13adeb6518cee5f88417660841142e830a81fe334380a953406a1305e8706b")
 R = bytes.fromhex("72cc4761dbd4c78f758931aa589d348d1ef874a7e303ede2f140dcf3e6aa4aac")
 CRED_R = bytes.fromhex("A2026008A101A5010202410A2001215820BBC34960526EA4D32E940CAD2A234148DDC21791A12AFBCBAC93622046DD44F02258204519E257236B2A0CE2023F0931F1F386CA7AFDA64FCDE0108C224C51EABF6072")
 CONTEXT = [0xa0, 0x11, 0x58, 0xfd, 0xb8, 0x20, 0x89, 0x0c, 0xd6, 0xbe, 0x16, 0x96, 0x02, 0xb8, 0xbc, 0xea]
 
 def test_gen_keys():
     priv, pub = lakers.p256_generate_key_pair()
@@ -17,33 +18,50 @@
     initiator = lakers.EdhocInitiator()
     message_1 = initiator.prepare_message_1(c_i=None, ead_1=None)
     assert type(message_1) == bytes
 
 def test_responder():
     responder = lakers.EdhocResponder(R, CRED_R)
 
-def test_handshake():
+def test_rpk_consruction():
+    # The main crednetials we use can be parsed as they are:
+    cred_r = lakers.CredentialRPK(CRED_R)
+
+    # We can also parse them on our own and construct an equivalent credential:
+    parsed_cred_r = cbor2.loads(CRED_R)
+    public_key = parsed_cred_r[8][1][-2]
+    kid = ord(parsed_cred_r[8][1][2])
+    cred_r_manual = lakers.CredentialRPK(CRED_R, public_key=public_key, kid=kid)
+
+    # No equality is useful, but the reprs are comprehensive
+    assert repr(cred_r_manual) == repr(cred_r)
+
+    # Both forms are accepted for constructing equivalent responders
+    _ = lakers.EdhocResponder(R, CRED_R)
+    _ = lakers.EdhocResponder(R, cred_r_manual)
+
+def _test_handshake(cred_r_transfer, cred_i_transfer):
     initiator = lakers.EdhocInitiator()
     responder = lakers.EdhocResponder(R, CRED_R)
 
     # initiator
     message_1 = initiator.prepare_message_1(c_i=None, ead_1=None)
 
     # responder
     _c_i, ead_1 = responder.process_message_1(message_1)
     assert ead_1 == None
-    message_2 = responder.prepare_message_2(lakers.CredentialTransfer.ByReference, None, ead_1)
+    message_2 = responder.prepare_message_2(cred_r_transfer, None, ead_1)
     assert type(message_2) == bytes
 
     # initiator
     c_r, id_cred_r, ead_2 = initiator.parse_message_2(message_2)
     assert ead_2 == None
     valid_cred_r = lakers.credential_check_or_fetch(id_cred_r, CRED_R)
     initiator.verify_message_2(I, CRED_I, valid_cred_r)
-    message_3, i_prk_out = initiator.prepare_message_3(lakers.CredentialTransfer.ByReference, None)
+    message_3, i_prk_out = initiator.prepare_message_3(cred_i_transfer, None)
     assert type(message_3) == bytes
 
     # responder
     id_cred_i, ead_3 = responder.parse_message_3(message_3)
     assert ead_3 == None
     valid_cred_i = lakers.credential_check_or_fetch(id_cred_i, CRED_I)
     r_prk_out = responder.verify_message_3(valid_cred_i)
@@ -69,7 +87,13 @@
     assert str(err.value) == "EDHOCError::ParsingError"
 
 def test_buffer_error():
     initiator = lakers.EdhocInitiator()
     with pytest.raises(ValueError) as err:
         _ = initiator.parse_message_2([1] * 1000)
     assert str(err.value) == "MessageBufferError::SliceTooLong"
+
+def test_handshake_byvalue_byreference():
+    _test_handshake(lakers.CredentialTransfer.ByValue, lakers.CredentialTransfer.ByReference)
+
+def test_handshake_byreference_byvalue():
+    _test_handshake(lakers.CredentialTransfer.ByReference, lakers.CredentialTransfer.ByValue)
```

### Comparing `lakers_python-0.3.0/Cargo.lock` & `lakers_python-0.3.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 dependencies = [
  "crypto-common",
  "generic-array 0.14.7",
 ]
 
 [[package]]
 name = "aes"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac1f845298e95f983ff1944b728ae08b8cebab80d684f0a832ed0fc74dfa27e2"
+checksum = "b169f7a6d4742236a0a00c541b845991d0ac43e546831af1249753ab4c3aa3a0"
 dependencies = [
  "cfg-if",
  "cipher",
  "cpufeatures",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "ansi_term"
 version = "0.12.1"
@@ -86,23 +86,23 @@
  "hermit-abi 0.1.19",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -145,32 +145,32 @@
  "rustc-hash",
  "shlex",
  "which",
 ]
 
 [[package]]
 name = "bindgen"
-version = "0.69.2"
+version = "0.69.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4c69fae65a523209d34240b60abe0c42d33d1045d445c0839d8a4894a736e2d"
+checksum = "a00dc851838a2120612785d195287475a3ac45514741da670b735818822129a0"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cexpr",
  "clang-sys",
+ "itertools",
  "lazy_static",
  "lazycell",
  "log",
- "peeking_take_while",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.48",
+ "syn 2.0.64",
  "which",
 ]
 
 [[package]]
 name = "bitfield"
 version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -180,17 +180,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
@@ -201,17 +201,17 @@
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cbindgen"
 version = "0.24.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b922faaf31122819ec80c4047cc684c6979a087366c069611e33649bf98e18d"
 dependencies = [
@@ -226,20 +226,17 @@
  "syn 1.0.109",
  "tempfile",
  "toml",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
-dependencies = [
- "libc",
-]
+checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
 
 [[package]]
 name = "ccm"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ae3c82e4355234767756212c570e29833699ab63e6ffd161887314cc5b43847"
 dependencies = [
@@ -262,17 +259,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
+checksum = "05afea1e0a06c9be33d539b876f1ce3692f4afea2cb41f740e7743225ed1c757"
 
 [[package]]
 name = "cipher"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
 dependencies = [
@@ -314,15 +311,15 @@
 dependencies = [
  "atty",
  "bitflags 1.3.2",
  "clap_lex",
  "indexmap",
  "strsim 0.10.0",
  "termcolor",
- "textwrap 0.16.0",
+ "textwrap 0.16.1",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
@@ -343,15 +340,15 @@
 name = "coap"
 version = "0.1.0"
 dependencies = [
  "coap 0.13.0",
  "coap-handler",
  "coap-handler-implementations",
  "coap-lite",
- "coap-message",
+ "coap-message 0.3.1",
  "coap-message-utils",
  "coap-numbers",
  "embedded-nal",
  "embedded-nal-minimal-coapserver",
  "hexlit",
  "lakers",
  "lakers-crypto",
@@ -383,86 +380,95 @@
 
 [[package]]
 name = "coap-handler"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8600ae8e54c9be6e0c5273fad0503e12f827742e4e3fea5a521412478d603b72"
 dependencies = [
- "coap-message",
+ "coap-message 0.3.1",
  "coap-numbers",
 ]
 
 [[package]]
 name = "coap-handler-implementations"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f2735f53da500caae442466ba2126d62458e86116ec1e273919880410f7e187b"
 dependencies = [
  "ciborium-io",
  "coap-handler",
- "coap-message",
+ "coap-message 0.3.1",
  "coap-message-utils",
  "coap-numbers",
  "crc",
  "document-features",
  "embedded-io",
  "minicbor",
  "serde",
  "serde_cbor",
  "windowed-infinity",
 ]
 
 [[package]]
 name = "coap-lite"
-version = "0.11.3"
+version = "0.11.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25ca11cbc756cf12eb24824285dbe36d97e4cfea404aaa1240477f3ae091f779"
+checksum = "1d72f4fbcb650652c4b7d980390cf8af49a738422ac66718bd516ec3430b83a6"
 dependencies = [
+ "coap-message 0.2.3",
+ "coap-message 0.3.1",
  "lru_time_cache",
 ]
 
 [[package]]
 name = "coap-message"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7cc888e15f6be910b58fda4f056f673f58fb9348ea45da014283a14e6d2b58ec"
+
+[[package]]
+name = "coap-message"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae18782d02e6afdfcfaf48eb7ec591b0cae57b67b637441a490752d4a57db02f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "coap-message-implementations"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "34293ae8447d52635184f556489bad7fa564d94cde3d00b170e2727964bc3645"
+checksum = "65b11a790471777e78eb68d908d300034b07a98bc43378a6b81159948c1361cd"
 dependencies = [
- "coap-message",
+ "coap-message 0.3.1",
  "coap-message-utils",
  "coap-numbers",
+ "document-features",
  "heapless 0.5.6",
 ]
 
 [[package]]
 name = "coap-message-utils"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ebb49f08ced17ea3a47a9206d99186849665854cea1fd064509008ed0cdfc4b"
+checksum = "d57c1e386dfabcc211aefd8d0cc64e8fa6ebc799736ee639a888e0e2af2734ea"
 dependencies = [
- "coap-message",
+ "coap-message 0.3.1",
  "coap-numbers",
  "document-features",
  "heapless 0.5.6",
  "minicbor",
 ]
 
 [[package]]
 name = "coap-numbers"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e766be4563107bc11c281c017ab922c3f3079345c9aa0fe747b4f9abc13411ac"
+checksum = "6d78a5634393ab2c11d173d66107200a730e200a3b3ca063c344d4459c90a5f9"
 
 [[package]]
 name = "const-oid"
 version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c2459377285ad874054d797f3ccebf984978aa39129f6eafde5cdc8315b612f8"
 
@@ -477,17 +483,17 @@
  "critical-section",
  "embedded-hal",
  "volatile-register",
 ]
 
 [[package]]
 name = "cortex-m-rt"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee84e813d593101b1723e13ec38b6ab6abbdbaaa4546553f5395ed274079ddb1"
+checksum = "2722f5b7d6ea8583cffa4d247044e280ccbb9fe501bed56552e2ba48b02d5f3d"
 dependencies = [
  "cortex-m-rt-macros",
 ]
 
 [[package]]
 name = "cortex-m-rt-macros"
 version = "0.7.0"
@@ -515,17 +521,17 @@
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc"
-version = "3.0.1"
+version = "3.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86ec7a15cbe22e59248fc7eadb1907dab5ba09372595da4d73dd805ed4417dfe"
+checksum = "69e6e4d7b33a94f0991c26729976b10ebde1d34c3ee82408fb536164fa10d636"
 dependencies = [
  "crc-catalog",
 ]
 
 [[package]]
 name = "crc-catalog"
 version = "2.4.0"
@@ -567,17 +573,17 @@
 checksum = "0369ee1ad671834580515889b80f2ea915f23b8be8d0daa4bbaf2ac5c7590835"
 dependencies = [
  "cipher",
 ]
 
 [[package]]
 name = "der"
-version = "0.7.8"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fffa369a668c8af7dbf8b5e56c9f744fbd399949ed171606040001947de40b1c"
+checksum = "f55bf8e7b65898637379c1b74eb1551107c8294ed26d855ceb9fd1a09cfc9bc0"
 dependencies = [
  "const-oid",
  "zeroize",
 ]
 
 [[package]]
 name = "digest"
@@ -597,17 +603,17 @@
 checksum = "ef5282ad69563b5fc40319526ba27e0e7363d552a896f0297d54f767717f9b95"
 dependencies = [
  "litrs",
 ]
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "elliptic-curve"
 version = "0.13.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b5e6043086bf7973472e0c7dff2142ea0b680d30e18d9cc40f267efbf222bd47"
 dependencies = [
@@ -664,15 +670,15 @@
 [[package]]
 name = "embedded-nal-minimal-coapserver"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6e7e827cbc4f6bf46b9973946396e7e3dae3e0d34aa8e560924b7d62dbcaf55"
 dependencies = [
  "coap-handler",
- "coap-message",
+ "coap-message 0.3.1",
  "coap-message-implementations",
  "coap-numbers",
  "embedded-nal",
  "heapless 0.5.6",
  "num-derive",
  "num-traits",
 ]
@@ -688,27 +694,27 @@
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "ff"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ded41244b729663b1e574f1b4fb731469f69f79c17667b5d776b16cda0479449"
 dependencies = [
@@ -777,15 +783,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.64",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -841,17 +847,17 @@
  "typenum",
  "version_check",
  "zeroize",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -875,17 +881,17 @@
  "ff",
  "rand_core",
  "subtle",
 ]
 
 [[package]]
 name = "half"
-version = "1.8.2"
+version = "1.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
+checksum = "1b43ede17f21864e81be2fa654110bf1e793774238d86ef8555c37e6519c0403"
 
 [[package]]
 name = "hash32"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4041af86e63ac4298ce40e5cca669066e75b6f1aa3390fe2561ffa5e1d9f4cc"
 dependencies = [
@@ -945,17 +951,23 @@
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.3"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
+
+[[package]]
+name = "hex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "hexlit"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b6e75c860d4216ac53f9ac88b25c99eaedba075b3a7b2ed31f2adc51a74fffd"
 
@@ -1010,103 +1022,112 @@
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "inout"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
 dependencies = [
  "generic-array 0.14.7",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "lakers"
-version = "0.5.1"
+version = "0.6.0"
 dependencies = [
  "hexlit",
  "lakers-crypto",
  "lakers-ead-authz",
  "lakers-shared",
 ]
 
 [[package]]
 name = "lakers-c"
-version = "0.5.1"
+version = "0.6.0"
 dependencies = [
  "cbindgen",
  "critical-section",
  "embedded-alloc",
  "hexlit",
  "lakers",
  "lakers-crypto",
  "lakers-ead-authz",
  "panic-semihosting",
 ]
 
 [[package]]
 name = "lakers-crypto"
-version = "0.5.1"
+version = "0.6.0"
 dependencies = [
  "hexlit",
  "lakers-crypto-cryptocell310",
  "lakers-crypto-psa",
  "lakers-crypto-rustcrypto",
  "lakers-shared",
  "rand_core",
  "rstest",
 ]
 
 [[package]]
 name = "lakers-crypto-cryptocell310"
-version = "0.5.1"
+version = "0.6.0"
 dependencies = [
- "bindgen 0.69.2",
+ "bindgen 0.69.4",
  "lakers-shared",
 ]
 
 [[package]]
 name = "lakers-crypto-psa"
-version = "0.5.1"
+version = "0.6.0"
 dependencies = [
  "lakers-shared",
  "psa-crypto",
 ]
 
 [[package]]
 name = "lakers-crypto-rustcrypto"
-version = "0.5.1"
+version = "0.6.0"
 dependencies = [
  "aead",
  "aes",
  "ccm",
  "hkdf",
  "lakers-shared",
  "p256",
  "rand_core",
  "sha2",
 ]
 
 [[package]]
 name = "lakers-ead-authz"
-version = "0.5.1"
+version = "0.6.0"
 dependencies = [
  "hexlit",
  "lakers-crypto",
  "lakers-shared",
 ]
 
 [[package]]
@@ -1123,27 +1144,28 @@
  "lakers-ead-authz",
  "panic-semihosting",
  "rtt-target",
 ]
 
 [[package]]
 name = "lakers-python"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "lakers",
  "lakers-crypto",
  "lakers-ead-authz",
  "lakers-shared",
  "pyo3",
 ]
 
 [[package]]
 name = "lakers-shared"
-version = "0.5.1"
+version = "0.6.0"
 dependencies = [
+ "hex",
  "hexlit",
  "pyo3",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -1154,79 +1176,79 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.152"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libloading"
-version = "0.8.1"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c571b676ddfc9a8c12f1f3d3085a7b163966a8fd8098a90640953ce5f6170161"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-sys 0.48.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "linked_list_allocator"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9afa463f5405ee81cdb9cc2baf37e08ec7e4c8209442b5d72c04cfb2cd6e6286"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.13"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "litrs"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4ce301924b7887e9d637144fdade93f9dfff9b60981d4ac161db09720d39aa5"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "lru_time_cache"
 version = "0.11.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9106e1d747ffd48e6be5bb2d97fa706ed25b144fbee4d5c02eae110cd8d6badd"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "minicbor"
 version = "0.19.1"
@@ -1237,17 +1259,17 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.8"
@@ -1300,28 +1322,28 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.17"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.3.3",
+ "hermit-abi 0.3.9",
  "libc",
 ]
 
 [[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1360,33 +1382,33 @@
 dependencies = [
  "cortex-m",
  "cortex-m-semihosting",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
@@ -1395,48 +1417,54 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "prettyplease"
-version = "0.2.16"
+version = "0.2.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a41cf62165e97c7f814d2221421dbb9afcbcdb0a88068e5ea206e19951c2cbb5"
+checksum = "5f12335488a2f3b0a83b14edad48dca9879ce89b2edd10e80237e4e852dd645e"
 dependencies = [
  "proc-macro2",
- "syn 2.0.48",
+ "syn 2.0.64",
 ]
 
 [[package]]
 name = "primeorder"
 version = "0.13.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "353e1ca18966c16d9deb1c69278edbc5f194139612772bd9537af60ac231e1e6"
 dependencies = [
  "elliptic-curve",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.76"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95fc56cda0b5c3325f5fbbd7ff9fda9e02bb00bb3dac51252d2f1bfa1cb8cc8c"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psa-crypto"
 version = "0.9.2"
@@ -1457,78 +1485,80 @@
  "cc",
  "cmake",
  "walkdir",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.64",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.64",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
@@ -1536,49 +1566,49 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.2"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.3"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rstest"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2288c66aeafe3b2ed227c981f364f9968fa952ef0b30e84ada4486e7ee24d00a"
 dependencies = [
@@ -1597,17 +1627,17 @@
 dependencies = [
  "cortex-m",
  "ufmt-write",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
@@ -1622,35 +1652,35 @@
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
- "semver 1.0.21",
+ "semver 1.0.23",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.30"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "322394588aaf33c24007e8bb3238ee3e4c5c09c084ab32bc73890b99ff326bca"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.16"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -1683,29 +1713,29 @@
 checksum = "1d7eb9ef2c18661902cc47e535f9bc51b78acd254da71d375c2f6720d9a40403"
 dependencies = [
  "semver-parser",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.21"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b97ed7a9823b74f99c7742f5336af7be5ecd3eeafcb1507d1fa93347b1d589b0"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
 [[package]]
 name = "serde"
-version = "1.0.195"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63261df402c67811e9ac6def069e4786148c4563f4b50fd4bf30aa370d626b02"
+checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_cbor"
 version = "0.11.2"
@@ -1714,28 +1744,28 @@
 dependencies = [
  "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.195"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46fe8f8603d81ba86327b23a2e9cdf49e1255fb94a4c5f297f6ee0547178ea2c"
+checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.64",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.111"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176e46fa42316f18edd598015a5166857fc835ec732f5215eac6b7bdbf0a84f4"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1747,23 +1777,23 @@
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "shlex"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7cee0529a6d40f580e7a5e6c495c8fbfe21b7b52795ed4bb5e62cdf92bc6380"
+checksum = "0fda2ff0d084019ba4d7c6f371c95d8fd75ce3524c3cb8fb653a3023f6323e64"
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "slab"
 version = "0.4.9"
@@ -1771,26 +1801,26 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.12.0"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2593d31f82ead8df961d8bd23a64c2ccf2eb5dd34b0a34bfb4dd54011c72009e"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.5"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
@@ -1840,38 +1870,37 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.48"
+version = "2.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
+checksum = "7ad3dee41f36859875573074334c200d1add8e4a87bb37113ebd31d926b7b11f"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tempfile"
-version = "3.9.0"
+version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01ce4141aa927a6d1bd34a041795abd0db1cccba5d5f24b009f694bdf3a1f3fa"
+checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
- "redox_syscall",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.4.1"
@@ -1888,17 +1917,17 @@
 checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
 dependencies = [
  "unicode-width",
 ]
 
 [[package]]
 name = "textwrap"
-version = "0.16.0"
+version = "0.16.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
+checksum = "23d434d3f8967a09480fb04132ebe0a3e088c173e6d0ee7897abbdf4eab0f8b9"
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
@@ -1934,22 +1963,22 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.64",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.14"
+version = "0.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
+checksum = "267ac89e0bec6e691e5813911606935d77c476ff49024f98abcea3e7b15e37af"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
@@ -1985,38 +2014,38 @@
 name = "ufmt-write"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e87a2ed6b42ec5e28cc3b94c09982969e9227600b2e3dcbc1db927a84c06bd69"
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.14"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f2528f27a9eb2b21e69c95319b30bd0efd85d09c379741b0f78ea1d86be2416"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
@@ -2062,17 +2091,17 @@
 checksum = "de437e2a6208b014ab52972a27e59b33fa2920d3e00fe05026167a1c509d19cc"
 dependencies = [
  "vcell",
 ]
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
@@ -2106,19 +2135,19 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
@@ -2149,15 +2178,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2169,110 +2198,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
 dependencies = [
@@ -2283,9 +2319,9 @@
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.64",
 ]
```

### Comparing `lakers_python-0.3.0/Cargo.toml` & `lakers_python-0.3.1/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 # this needs to be explicitly set if using virtual manifests (like this).
 # We need this so dependency crates use it *in all cases*.
 # Specifically, `psa-crypto` merges build-dependency and regular dependency
 # features without this, causing forced "std" in downstream crate.
 resolver = "2"
 
 [workspace.package]
-version = "0.5.1"
+version = "0.6.0"
 repository = "https://github.com/openwsn-berkeley/lakers/"
 license = "BSD-3-Clause"
 readme = "shared/README.md"
 keywords = ["iot", "security", "protocol", "crypto", "edhoc"]
 categories = [ "no-std::no-alloc", "network-programming", "embedded" ]
 
 [workspace.dependencies]
 
-lakers-shared = { package = "lakers-shared", path = "shared/", version = "^0.5.1" }
+lakers-shared = { package = "lakers-shared", path = "shared/", version = "^0.6.0" }
 
-lakers-ead-authz = { package = "lakers-ead-authz", path = "ead/lakers-ead-authz/", version = "^0.5.1" }
+lakers-ead-authz = { package = "lakers-ead-authz", path = "ead/lakers-ead-authz/", version = "^0.6.0" }
 
 lakers-crypto = { path = "crypto/" }
 lakers-crypto-cryptocell310 = { path = "crypto/lakers-crypto-cryptocell310-sys/" }
 lakers-crypto-psa = { path = "crypto/lakers-crypto-psa/" }
-lakers-crypto-rustcrypto = { package = "lakers-crypto-rustcrypto", path = "crypto/lakers-crypto-rustcrypto/", version = "^0.5.1" }
+lakers-crypto-rustcrypto = { package = "lakers-crypto-rustcrypto", path = "crypto/lakers-crypto-rustcrypto/", version = "^0.6.0" }
 
-lakers = { package = "lakers", path = "lib/", version = "^0.5.1", default-features = false }
+lakers = { package = "lakers", path = "lib/", version = "^0.6.0", default-features = false }
 
 [patch.crates-io]
 psa-crypto = { git = "https://github.com/malishav/rust-psa-crypto", branch = "baremetal" }
```

