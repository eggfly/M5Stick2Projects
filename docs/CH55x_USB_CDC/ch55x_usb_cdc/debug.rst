                                      1 ;--------------------------------------------------------
                                      2 ; File Created by SDCC : free open source ANSI-C Compiler
                                      3 ; Version 3.8.0 #10562 (MINGW64)
                                      4 ;--------------------------------------------------------
                                      5 	.module debug
                                      6 	.optsdcc -mmcs51 --model-small
                                      7 	
                                      8 ;--------------------------------------------------------
                                      9 ; Public variables in this module
                                     10 ;--------------------------------------------------------
                                     11 	.globl _UIF_BUS_RST
                                     12 	.globl _UIF_DETECT
                                     13 	.globl _UIF_TRANSFER
                                     14 	.globl _UIF_SUSPEND
                                     15 	.globl _UIF_HST_SOF
                                     16 	.globl _UIF_FIFO_OV
                                     17 	.globl _U_SIE_FREE
                                     18 	.globl _U_TOG_OK
                                     19 	.globl _U_IS_NAK
                                     20 	.globl _ADC_CHAN0
                                     21 	.globl _ADC_CHAN1
                                     22 	.globl _CMP_CHAN
                                     23 	.globl _ADC_START
                                     24 	.globl _ADC_IF
                                     25 	.globl _CMP_IF
                                     26 	.globl _CMPO
                                     27 	.globl _U1RI
                                     28 	.globl _U1TI
                                     29 	.globl _U1RB8
                                     30 	.globl _U1TB8
                                     31 	.globl _U1REN
                                     32 	.globl _U1SMOD
                                     33 	.globl _U1SM0
                                     34 	.globl _S0_R_FIFO
                                     35 	.globl _S0_T_FIFO
                                     36 	.globl _S0_FREE
                                     37 	.globl _S0_IF_BYTE
                                     38 	.globl _S0_IF_FIRST
                                     39 	.globl _S0_IF_OV
                                     40 	.globl _S0_FST_ACT
                                     41 	.globl _CP_RL2
                                     42 	.globl _C_T2
                                     43 	.globl _TR2
                                     44 	.globl _EXEN2
                                     45 	.globl _TCLK
                                     46 	.globl _RCLK
                                     47 	.globl _EXF2
                                     48 	.globl _CAP1F
                                     49 	.globl _TF2
                                     50 	.globl _RI
                                     51 	.globl _TI
                                     52 	.globl _RB8
                                     53 	.globl _TB8
                                     54 	.globl _REN
                                     55 	.globl _SM2
                                     56 	.globl _SM1
                                     57 	.globl _SM0
                                     58 	.globl _IT0
                                     59 	.globl _IE0
                                     60 	.globl _IT1
                                     61 	.globl _IE1
                                     62 	.globl _TR0
                                     63 	.globl _TF0
                                     64 	.globl _TR1
                                     65 	.globl _TF1
                                     66 	.globl _RXD
                                     67 	.globl _PWM1_
                                     68 	.globl _TXD
                                     69 	.globl _PWM2_
                                     70 	.globl _AIN3
                                     71 	.globl _VBUS1
                                     72 	.globl _INT0
                                     73 	.globl _TXD1_
                                     74 	.globl _INT1
                                     75 	.globl _T0
                                     76 	.globl _RXD1_
                                     77 	.globl _PWM2
                                     78 	.globl _T1
                                     79 	.globl _UDP
                                     80 	.globl _UDM
                                     81 	.globl _TIN0
                                     82 	.globl _CAP1
                                     83 	.globl _T2
                                     84 	.globl _AIN0
                                     85 	.globl _VBUS2
                                     86 	.globl _TIN1
                                     87 	.globl _CAP2
                                     88 	.globl _T2EX
                                     89 	.globl _RXD_
                                     90 	.globl _TXD_
                                     91 	.globl _AIN1
                                     92 	.globl _UCC1
                                     93 	.globl _TIN2
                                     94 	.globl _SCS
                                     95 	.globl _CAP1_
                                     96 	.globl _T2_
                                     97 	.globl _AIN2
                                     98 	.globl _UCC2
                                     99 	.globl _TIN3
                                    100 	.globl _PWM1
                                    101 	.globl _MOSI
                                    102 	.globl _TIN4
                                    103 	.globl _RXD1
                                    104 	.globl _MISO
                                    105 	.globl _TIN5
                                    106 	.globl _TXD1
                                    107 	.globl _SCK
                                    108 	.globl _IE_SPI0
                                    109 	.globl _IE_TKEY
                                    110 	.globl _IE_USB
                                    111 	.globl _IE_ADC
                                    112 	.globl _IE_UART1
                                    113 	.globl _IE_PWMX
                                    114 	.globl _IE_GPIO
                                    115 	.globl _IE_WDOG
                                    116 	.globl _PX0
                                    117 	.globl _PT0
                                    118 	.globl _PX1
                                    119 	.globl _PT1
                                    120 	.globl _PS
                                    121 	.globl _PT2
                                    122 	.globl _PL_FLAG
                                    123 	.globl _PH_FLAG
                                    124 	.globl _EX0
                                    125 	.globl _ET0
                                    126 	.globl _EX1
                                    127 	.globl _ET1
                                    128 	.globl _ES
                                    129 	.globl _ET2
                                    130 	.globl _E_DIS
                                    131 	.globl _EA
                                    132 	.globl _P
                                    133 	.globl _F1
                                    134 	.globl _OV
                                    135 	.globl _RS0
                                    136 	.globl _RS1
                                    137 	.globl _F0
                                    138 	.globl _AC
                                    139 	.globl _CY
                                    140 	.globl _UEP1_DMA_H
                                    141 	.globl _UEP1_DMA_L
                                    142 	.globl _UEP1_DMA
                                    143 	.globl _UEP0_DMA_H
                                    144 	.globl _UEP0_DMA_L
                                    145 	.globl _UEP0_DMA
                                    146 	.globl _UEP2_3_MOD
                                    147 	.globl _UEP4_1_MOD
                                    148 	.globl _UEP3_DMA_H
                                    149 	.globl _UEP3_DMA_L
                                    150 	.globl _UEP3_DMA
                                    151 	.globl _UEP2_DMA_H
                                    152 	.globl _UEP2_DMA_L
                                    153 	.globl _UEP2_DMA
                                    154 	.globl _USB_DEV_AD
                                    155 	.globl _USB_CTRL
                                    156 	.globl _USB_INT_EN
                                    157 	.globl _UEP4_T_LEN
                                    158 	.globl _UEP4_CTRL
                                    159 	.globl _UEP0_T_LEN
                                    160 	.globl _UEP0_CTRL
                                    161 	.globl _USB_RX_LEN
                                    162 	.globl _USB_MIS_ST
                                    163 	.globl _USB_INT_ST
                                    164 	.globl _USB_INT_FG
                                    165 	.globl _UEP3_T_LEN
                                    166 	.globl _UEP3_CTRL
                                    167 	.globl _UEP2_T_LEN
                                    168 	.globl _UEP2_CTRL
                                    169 	.globl _UEP1_T_LEN
                                    170 	.globl _UEP1_CTRL
                                    171 	.globl _UDEV_CTRL
                                    172 	.globl _USB_C_CTRL
                                    173 	.globl _TKEY_DATH
                                    174 	.globl _TKEY_DATL
                                    175 	.globl _TKEY_DAT
                                    176 	.globl _TKEY_CTRL
                                    177 	.globl _ADC_DATA
                                    178 	.globl _ADC_CFG
                                    179 	.globl _ADC_CTRL
                                    180 	.globl _SBAUD1
                                    181 	.globl _SBUF1
                                    182 	.globl _SCON1
                                    183 	.globl _SPI0_SETUP
                                    184 	.globl _SPI0_CK_SE
                                    185 	.globl _SPI0_CTRL
                                    186 	.globl _SPI0_DATA
                                    187 	.globl _SPI0_STAT
                                    188 	.globl _PWM_CK_SE
                                    189 	.globl _PWM_CTRL
                                    190 	.globl _PWM_DATA1
                                    191 	.globl _PWM_DATA2
                                    192 	.globl _T2CAP1H
                                    193 	.globl _T2CAP1L
                                    194 	.globl _T2CAP1
                                    195 	.globl _TH2
                                    196 	.globl _TL2
                                    197 	.globl _T2COUNT
                                    198 	.globl _RCAP2H
                                    199 	.globl _RCAP2L
                                    200 	.globl _RCAP2
                                    201 	.globl _T2MOD
                                    202 	.globl _T2CON
                                    203 	.globl _SBUF
                                    204 	.globl _SCON
                                    205 	.globl _TH1
                                    206 	.globl _TH0
                                    207 	.globl _TL1
                                    208 	.globl _TL0
                                    209 	.globl _TMOD
                                    210 	.globl _TCON
                                    211 	.globl _XBUS_AUX
                                    212 	.globl _PIN_FUNC
                                    213 	.globl _P3_DIR_PU
                                    214 	.globl _P3_MOD_OC
                                    215 	.globl _P3
                                    216 	.globl _P2
                                    217 	.globl _P1_DIR_PU
                                    218 	.globl _P1_MOD_OC
                                    219 	.globl _P1
                                    220 	.globl _ROM_CTRL
                                    221 	.globl _ROM_DATA_H
                                    222 	.globl _ROM_DATA_L
                                    223 	.globl _ROM_DATA
                                    224 	.globl _ROM_ADDR_H
                                    225 	.globl _ROM_ADDR_L
                                    226 	.globl _ROM_ADDR
                                    227 	.globl _GPIO_IE
                                    228 	.globl _IP_EX
                                    229 	.globl _IE_EX
                                    230 	.globl _IP
                                    231 	.globl _IE
                                    232 	.globl _WDOG_COUNT
                                    233 	.globl _RESET_KEEP
                                    234 	.globl _WAKE_CTRL
                                    235 	.globl _CLOCK_CFG
                                    236 	.globl _PCON
                                    237 	.globl _GLOBAL_CFG
                                    238 	.globl _SAFE_MOD
                                    239 	.globl _DPH
                                    240 	.globl _DPL
                                    241 	.globl _SP
                                    242 	.globl _B
                                    243 	.globl _ACC
                                    244 	.globl _PSW
                                    245 	.globl _CfgFsys
                                    246 	.globl _mDelayuS
                                    247 	.globl _mDelaymS
                                    248 	.globl _CH554UART0Alter
                                    249 	.globl _mInitSTDIO
                                    250 	.globl _CH554UART0RcvByte
                                    251 	.globl _CH554UART0SendByte
                                    252 	.globl _putchar
                                    253 	.globl _getchar
                                    254 	.globl _CH554UART1Alter
                                    255 	.globl _UART1Setup
                                    256 	.globl _CH554UART1RcvByte
                                    257 	.globl _CH554UART1SendByte
                                    258 	.globl _CH554WDTModeSelect
                                    259 	.globl _CH554WDTFeed
                                    260 ;--------------------------------------------------------
                                    261 ; special function registers
                                    262 ;--------------------------------------------------------
                                    263 	.area RSEG    (ABS,DATA)
      000000                        264 	.org 0x0000
                           0000D0   265 _PSW	=	0x00d0
                           0000E0   266 _ACC	=	0x00e0
                           0000F0   267 _B	=	0x00f0
                           000081   268 _SP	=	0x0081
                           000082   269 _DPL	=	0x0082
                           000083   270 _DPH	=	0x0083
                           0000A1   271 _SAFE_MOD	=	0x00a1
                           0000B1   272 _GLOBAL_CFG	=	0x00b1
                           000087   273 _PCON	=	0x0087
                           0000B9   274 _CLOCK_CFG	=	0x00b9
                           0000A9   275 _WAKE_CTRL	=	0x00a9
                           0000FE   276 _RESET_KEEP	=	0x00fe
                           0000FF   277 _WDOG_COUNT	=	0x00ff
                           0000A8   278 _IE	=	0x00a8
                           0000B8   279 _IP	=	0x00b8
                           0000E8   280 _IE_EX	=	0x00e8
                           0000E9   281 _IP_EX	=	0x00e9
                           0000C7   282 _GPIO_IE	=	0x00c7
                           008584   283 _ROM_ADDR	=	0x8584
                           000084   284 _ROM_ADDR_L	=	0x0084
                           000085   285 _ROM_ADDR_H	=	0x0085
                           008F8E   286 _ROM_DATA	=	0x8f8e
                           00008E   287 _ROM_DATA_L	=	0x008e
                           00008F   288 _ROM_DATA_H	=	0x008f
                           000086   289 _ROM_CTRL	=	0x0086
                           000090   290 _P1	=	0x0090
                           000092   291 _P1_MOD_OC	=	0x0092
                           000093   292 _P1_DIR_PU	=	0x0093
                           0000A0   293 _P2	=	0x00a0
                           0000B0   294 _P3	=	0x00b0
                           000096   295 _P3_MOD_OC	=	0x0096
                           000097   296 _P3_DIR_PU	=	0x0097
                           0000C6   297 _PIN_FUNC	=	0x00c6
                           0000A2   298 _XBUS_AUX	=	0x00a2
                           000088   299 _TCON	=	0x0088
                           000089   300 _TMOD	=	0x0089
                           00008A   301 _TL0	=	0x008a
                           00008B   302 _TL1	=	0x008b
                           00008C   303 _TH0	=	0x008c
                           00008D   304 _TH1	=	0x008d
                           000098   305 _SCON	=	0x0098
                           000099   306 _SBUF	=	0x0099
                           0000C8   307 _T2CON	=	0x00c8
                           0000C9   308 _T2MOD	=	0x00c9
                           00CBCA   309 _RCAP2	=	0xcbca
                           0000CA   310 _RCAP2L	=	0x00ca
                           0000CB   311 _RCAP2H	=	0x00cb
                           00CDCC   312 _T2COUNT	=	0xcdcc
                           0000CC   313 _TL2	=	0x00cc
                           0000CD   314 _TH2	=	0x00cd
                           00CFCE   315 _T2CAP1	=	0xcfce
                           0000CE   316 _T2CAP1L	=	0x00ce
                           0000CF   317 _T2CAP1H	=	0x00cf
                           00009B   318 _PWM_DATA2	=	0x009b
                           00009C   319 _PWM_DATA1	=	0x009c
                           00009D   320 _PWM_CTRL	=	0x009d
                           00009E   321 _PWM_CK_SE	=	0x009e
                           0000F8   322 _SPI0_STAT	=	0x00f8
                           0000F9   323 _SPI0_DATA	=	0x00f9
                           0000FA   324 _SPI0_CTRL	=	0x00fa
                           0000FB   325 _SPI0_CK_SE	=	0x00fb
                           0000FC   326 _SPI0_SETUP	=	0x00fc
                           0000C0   327 _SCON1	=	0x00c0
                           0000C1   328 _SBUF1	=	0x00c1
                           0000C2   329 _SBAUD1	=	0x00c2
                           000080   330 _ADC_CTRL	=	0x0080
                           00009A   331 _ADC_CFG	=	0x009a
                           00009F   332 _ADC_DATA	=	0x009f
                           0000C3   333 _TKEY_CTRL	=	0x00c3
                           00C5C4   334 _TKEY_DAT	=	0xc5c4
                           0000C4   335 _TKEY_DATL	=	0x00c4
                           0000C5   336 _TKEY_DATH	=	0x00c5
                           000091   337 _USB_C_CTRL	=	0x0091
                           0000D1   338 _UDEV_CTRL	=	0x00d1
                           0000D2   339 _UEP1_CTRL	=	0x00d2
                           0000D3   340 _UEP1_T_LEN	=	0x00d3
                           0000D4   341 _UEP2_CTRL	=	0x00d4
                           0000D5   342 _UEP2_T_LEN	=	0x00d5
                           0000D6   343 _UEP3_CTRL	=	0x00d6
                           0000D7   344 _UEP3_T_LEN	=	0x00d7
                           0000D8   345 _USB_INT_FG	=	0x00d8
                           0000D9   346 _USB_INT_ST	=	0x00d9
                           0000DA   347 _USB_MIS_ST	=	0x00da
                           0000DB   348 _USB_RX_LEN	=	0x00db
                           0000DC   349 _UEP0_CTRL	=	0x00dc
                           0000DD   350 _UEP0_T_LEN	=	0x00dd
                           0000DE   351 _UEP4_CTRL	=	0x00de
                           0000DF   352 _UEP4_T_LEN	=	0x00df
                           0000E1   353 _USB_INT_EN	=	0x00e1
                           0000E2   354 _USB_CTRL	=	0x00e2
                           0000E3   355 _USB_DEV_AD	=	0x00e3
                           00E5E4   356 _UEP2_DMA	=	0xe5e4
                           0000E4   357 _UEP2_DMA_L	=	0x00e4
                           0000E5   358 _UEP2_DMA_H	=	0x00e5
                           00E7E6   359 _UEP3_DMA	=	0xe7e6
                           0000E6   360 _UEP3_DMA_L	=	0x00e6
                           0000E7   361 _UEP3_DMA_H	=	0x00e7
                           0000EA   362 _UEP4_1_MOD	=	0x00ea
                           0000EB   363 _UEP2_3_MOD	=	0x00eb
                           00EDEC   364 _UEP0_DMA	=	0xedec
                           0000EC   365 _UEP0_DMA_L	=	0x00ec
                           0000ED   366 _UEP0_DMA_H	=	0x00ed
                           00EFEE   367 _UEP1_DMA	=	0xefee
                           0000EE   368 _UEP1_DMA_L	=	0x00ee
                           0000EF   369 _UEP1_DMA_H	=	0x00ef
                                    370 ;--------------------------------------------------------
                                    371 ; special function bits
                                    372 ;--------------------------------------------------------
                                    373 	.area RSEG    (ABS,DATA)
      000000                        374 	.org 0x0000
                           0000D7   375 _CY	=	0x00d7
                           0000D6   376 _AC	=	0x00d6
                           0000D5   377 _F0	=	0x00d5
                           0000D4   378 _RS1	=	0x00d4
                           0000D3   379 _RS0	=	0x00d3
                           0000D2   380 _OV	=	0x00d2
                           0000D1   381 _F1	=	0x00d1
                           0000D0   382 _P	=	0x00d0
                           0000AF   383 _EA	=	0x00af
                           0000AE   384 _E_DIS	=	0x00ae
                           0000AD   385 _ET2	=	0x00ad
                           0000AC   386 _ES	=	0x00ac
                           0000AB   387 _ET1	=	0x00ab
                           0000AA   388 _EX1	=	0x00aa
                           0000A9   389 _ET0	=	0x00a9
                           0000A8   390 _EX0	=	0x00a8
                           0000BF   391 _PH_FLAG	=	0x00bf
                           0000BE   392 _PL_FLAG	=	0x00be
                           0000BD   393 _PT2	=	0x00bd
                           0000BC   394 _PS	=	0x00bc
                           0000BB   395 _PT1	=	0x00bb
                           0000BA   396 _PX1	=	0x00ba
                           0000B9   397 _PT0	=	0x00b9
                           0000B8   398 _PX0	=	0x00b8
                           0000EF   399 _IE_WDOG	=	0x00ef
                           0000EE   400 _IE_GPIO	=	0x00ee
                           0000ED   401 _IE_PWMX	=	0x00ed
                           0000EC   402 _IE_UART1	=	0x00ec
                           0000EB   403 _IE_ADC	=	0x00eb
                           0000EA   404 _IE_USB	=	0x00ea
                           0000E9   405 _IE_TKEY	=	0x00e9
                           0000E8   406 _IE_SPI0	=	0x00e8
                           000097   407 _SCK	=	0x0097
                           000097   408 _TXD1	=	0x0097
                           000097   409 _TIN5	=	0x0097
                           000096   410 _MISO	=	0x0096
                           000096   411 _RXD1	=	0x0096
                           000096   412 _TIN4	=	0x0096
                           000095   413 _MOSI	=	0x0095
                           000095   414 _PWM1	=	0x0095
                           000095   415 _TIN3	=	0x0095
                           000095   416 _UCC2	=	0x0095
                           000095   417 _AIN2	=	0x0095
                           000094   418 _T2_	=	0x0094
                           000094   419 _CAP1_	=	0x0094
                           000094   420 _SCS	=	0x0094
                           000094   421 _TIN2	=	0x0094
                           000094   422 _UCC1	=	0x0094
                           000094   423 _AIN1	=	0x0094
                           000093   424 _TXD_	=	0x0093
                           000092   425 _RXD_	=	0x0092
                           000091   426 _T2EX	=	0x0091
                           000091   427 _CAP2	=	0x0091
                           000091   428 _TIN1	=	0x0091
                           000091   429 _VBUS2	=	0x0091
                           000091   430 _AIN0	=	0x0091
                           000090   431 _T2	=	0x0090
                           000090   432 _CAP1	=	0x0090
                           000090   433 _TIN0	=	0x0090
                           0000B7   434 _UDM	=	0x00b7
                           0000B6   435 _UDP	=	0x00b6
                           0000B5   436 _T1	=	0x00b5
                           0000B4   437 _PWM2	=	0x00b4
                           0000B4   438 _RXD1_	=	0x00b4
                           0000B4   439 _T0	=	0x00b4
                           0000B3   440 _INT1	=	0x00b3
                           0000B2   441 _TXD1_	=	0x00b2
                           0000B2   442 _INT0	=	0x00b2
                           0000B2   443 _VBUS1	=	0x00b2
                           0000B2   444 _AIN3	=	0x00b2
                           0000B1   445 _PWM2_	=	0x00b1
                           0000B1   446 _TXD	=	0x00b1
                           0000B0   447 _PWM1_	=	0x00b0
                           0000B0   448 _RXD	=	0x00b0
                           00008F   449 _TF1	=	0x008f
                           00008E   450 _TR1	=	0x008e
                           00008D   451 _TF0	=	0x008d
                           00008C   452 _TR0	=	0x008c
                           00008B   453 _IE1	=	0x008b
                           00008A   454 _IT1	=	0x008a
                           000089   455 _IE0	=	0x0089
                           000088   456 _IT0	=	0x0088
                           00009F   457 _SM0	=	0x009f
                           00009E   458 _SM1	=	0x009e
                           00009D   459 _SM2	=	0x009d
                           00009C   460 _REN	=	0x009c
                           00009B   461 _TB8	=	0x009b
                           00009A   462 _RB8	=	0x009a
                           000099   463 _TI	=	0x0099
                           000098   464 _RI	=	0x0098
                           0000CF   465 _TF2	=	0x00cf
                           0000CF   466 _CAP1F	=	0x00cf
                           0000CE   467 _EXF2	=	0x00ce
                           0000CD   468 _RCLK	=	0x00cd
                           0000CC   469 _TCLK	=	0x00cc
                           0000CB   470 _EXEN2	=	0x00cb
                           0000CA   471 _TR2	=	0x00ca
                           0000C9   472 _C_T2	=	0x00c9
                           0000C8   473 _CP_RL2	=	0x00c8
                           0000FF   474 _S0_FST_ACT	=	0x00ff
                           0000FE   475 _S0_IF_OV	=	0x00fe
                           0000FD   476 _S0_IF_FIRST	=	0x00fd
                           0000FC   477 _S0_IF_BYTE	=	0x00fc
                           0000FB   478 _S0_FREE	=	0x00fb
                           0000FA   479 _S0_T_FIFO	=	0x00fa
                           0000F8   480 _S0_R_FIFO	=	0x00f8
                           0000C7   481 _U1SM0	=	0x00c7
                           0000C5   482 _U1SMOD	=	0x00c5
                           0000C4   483 _U1REN	=	0x00c4
                           0000C3   484 _U1TB8	=	0x00c3
                           0000C2   485 _U1RB8	=	0x00c2
                           0000C1   486 _U1TI	=	0x00c1
                           0000C0   487 _U1RI	=	0x00c0
                           000087   488 _CMPO	=	0x0087
                           000086   489 _CMP_IF	=	0x0086
                           000085   490 _ADC_IF	=	0x0085
                           000084   491 _ADC_START	=	0x0084
                           000083   492 _CMP_CHAN	=	0x0083
                           000081   493 _ADC_CHAN1	=	0x0081
                           000080   494 _ADC_CHAN0	=	0x0080
                           0000DF   495 _U_IS_NAK	=	0x00df
                           0000DE   496 _U_TOG_OK	=	0x00de
                           0000DD   497 _U_SIE_FREE	=	0x00dd
                           0000DC   498 _UIF_FIFO_OV	=	0x00dc
                           0000DB   499 _UIF_HST_SOF	=	0x00db
                           0000DA   500 _UIF_SUSPEND	=	0x00da
                           0000D9   501 _UIF_TRANSFER	=	0x00d9
                           0000D8   502 _UIF_DETECT	=	0x00d8
                           0000D8   503 _UIF_BUS_RST	=	0x00d8
                                    504 ;--------------------------------------------------------
                                    505 ; overlayable register banks
                                    506 ;--------------------------------------------------------
                                    507 	.area REG_BANK_0	(REL,OVR,DATA)
      000000                        508 	.ds 8
                                    509 ;--------------------------------------------------------
                                    510 ; internal ram data
                                    511 ;--------------------------------------------------------
                                    512 	.area DSEG    (DATA)
      000019                        513 _mInitSTDIO_x_65536_17:
      000019                        514 	.ds 4
      00001D                        515 _mInitSTDIO_x2_65536_17:
      00001D                        516 	.ds 1
                                    517 ;--------------------------------------------------------
                                    518 ; overlayable items in internal ram 
                                    519 ;--------------------------------------------------------
                                    520 	.area	OSEG    (OVR,DATA)
                                    521 	.area	OSEG    (OVR,DATA)
                                    522 	.area	OSEG    (OVR,DATA)
                                    523 	.area	OSEG    (OVR,DATA)
                                    524 	.area	OSEG    (OVR,DATA)
                                    525 	.area	OSEG    (OVR,DATA)
                                    526 ;--------------------------------------------------------
                                    527 ; indirectly addressable internal ram data
                                    528 ;--------------------------------------------------------
                                    529 	.area ISEG    (DATA)
                                    530 ;--------------------------------------------------------
                                    531 ; absolute internal ram data
                                    532 ;--------------------------------------------------------
                                    533 	.area IABS    (ABS,DATA)
                                    534 	.area IABS    (ABS,DATA)
                                    535 ;--------------------------------------------------------
                                    536 ; bit data
                                    537 ;--------------------------------------------------------
                                    538 	.area BSEG    (BIT)
                                    539 ;--------------------------------------------------------
                                    540 ; paged external ram data
                                    541 ;--------------------------------------------------------
                                    542 	.area PSEG    (PAG,XDATA)
                                    543 ;--------------------------------------------------------
                                    544 ; external ram data
                                    545 ;--------------------------------------------------------
                                    546 	.area XSEG    (XDATA)
                                    547 ;--------------------------------------------------------
                                    548 ; absolute external ram data
                                    549 ;--------------------------------------------------------
                                    550 	.area XABS    (ABS,XDATA)
                                    551 ;--------------------------------------------------------
                                    552 ; external initialized ram data
                                    553 ;--------------------------------------------------------
                                    554 	.area XISEG   (XDATA)
                                    555 	.area HOME    (CODE)
                                    556 	.area GSINIT0 (CODE)
                                    557 	.area GSINIT1 (CODE)
                                    558 	.area GSINIT2 (CODE)
                                    559 	.area GSINIT3 (CODE)
                                    560 	.area GSINIT4 (CODE)
                                    561 	.area GSINIT5 (CODE)
                                    562 	.area GSINIT  (CODE)
                                    563 	.area GSFINAL (CODE)
                                    564 	.area CSEG    (CODE)
                                    565 ;--------------------------------------------------------
                                    566 ; global & static initialisations
                                    567 ;--------------------------------------------------------
                                    568 	.area HOME    (CODE)
                                    569 	.area GSINIT  (CODE)
                                    570 	.area GSFINAL (CODE)
                                    571 	.area GSINIT  (CODE)
                                    572 ;--------------------------------------------------------
                                    573 ; Home
                                    574 ;--------------------------------------------------------
                                    575 	.area HOME    (CODE)
                                    576 	.area HOME    (CODE)
                                    577 ;--------------------------------------------------------
                                    578 ; code
                                    579 ;--------------------------------------------------------
                                    580 	.area CSEG    (CODE)
                                    581 ;------------------------------------------------------------
                                    582 ;Allocation info for local variables in function 'CfgFsys'
                                    583 ;------------------------------------------------------------
                                    584 ;	../include/debug.c:27: void	CfgFsys( )  
                                    585 ;	-----------------------------------------
                                    586 ;	 function CfgFsys
                                    587 ;	-----------------------------------------
      000FFC                        588 _CfgFsys:
                           000007   589 	ar7 = 0x07
                           000006   590 	ar6 = 0x06
                           000005   591 	ar5 = 0x05
                           000004   592 	ar4 = 0x04
                           000003   593 	ar3 = 0x03
                           000002   594 	ar2 = 0x02
                           000001   595 	ar1 = 0x01
                           000000   596 	ar0 = 0x00
                                    597 ;	../include/debug.c:34: SAFE_MOD = 0x55;
      000FFC 75 A1 55         [24]  598 	mov	_SAFE_MOD,#0x55
                                    599 ;	../include/debug.c:35: SAFE_MOD = 0xAA;
      000FFF 75 A1 AA         [24]  600 	mov	_SAFE_MOD,#0xaa
                                    601 ;	../include/debug.c:42: CLOCK_CFG = CLOCK_CFG & ~ MASK_SYS_CK_SEL | 0x05;  // 16MHz	
      001002 74 F8            [12]  602 	mov	a,#0xf8
      001004 55 B9            [12]  603 	anl	a,_CLOCK_CFG
      001006 FF               [12]  604 	mov	r7,a
      001007 43 07 05         [24]  605 	orl	ar7,#0x05
      00100A 8F B9            [24]  606 	mov	_CLOCK_CFG,r7
                                    607 ;	../include/debug.c:57: SAFE_MOD = 0x00;
      00100C 75 A1 00         [24]  608 	mov	_SAFE_MOD,#0x00
                                    609 ;	../include/debug.c:58: }
      00100F 22               [24]  610 	ret
                                    611 ;------------------------------------------------------------
                                    612 ;Allocation info for local variables in function 'mDelayuS'
                                    613 ;------------------------------------------------------------
                                    614 ;n                         Allocated to registers 
                                    615 ;------------------------------------------------------------
                                    616 ;	../include/debug.c:69: void	mDelayuS( uint16_t n )  // 以uS为单位延时
                                    617 ;	-----------------------------------------
                                    618 ;	 function mDelayuS
                                    619 ;	-----------------------------------------
      001010                        620 _mDelayuS:
      001010 AE 82            [24]  621 	mov	r6,dpl
      001012 AF 83            [24]  622 	mov	r7,dph
                                    623 ;	../include/debug.c:82: while ( n ) {  // total = 12~13 Fsys cycles, 1uS @Fsys=12MHz
      001014                        624 00101$:
      001014 EE               [12]  625 	mov	a,r6
      001015 4F               [12]  626 	orl	a,r7
      001016 60 0D            [24]  627 	jz	00104$
                                    628 ;	../include/debug.c:83: ++ SAFE_MOD;  // 2 Fsys cycles, for higher Fsys, add operation here
      001018 05 A1            [12]  629 	inc	_SAFE_MOD
                                    630 ;	../include/debug.c:86: ++ SAFE_MOD;
      00101A 05 A1            [12]  631 	inc	_SAFE_MOD
                                    632 ;	../include/debug.c:89: ++ SAFE_MOD;
      00101C 05 A1            [12]  633 	inc	_SAFE_MOD
                                    634 ;	../include/debug.c:116: -- n;
      00101E 1E               [12]  635 	dec	r6
      00101F BE FF 01         [24]  636 	cjne	r6,#0xff,00116$
      001022 1F               [12]  637 	dec	r7
      001023                        638 00116$:
      001023 80 EF            [24]  639 	sjmp	00101$
      001025                        640 00104$:
                                    641 ;	../include/debug.c:118: }
      001025 22               [24]  642 	ret
                                    643 ;------------------------------------------------------------
                                    644 ;Allocation info for local variables in function 'mDelaymS'
                                    645 ;------------------------------------------------------------
                                    646 ;n                         Allocated to registers 
                                    647 ;------------------------------------------------------------
                                    648 ;	../include/debug.c:127: void	mDelaymS( uint16_t n )                                                  // 以mS为单位延时
                                    649 ;	-----------------------------------------
                                    650 ;	 function mDelaymS
                                    651 ;	-----------------------------------------
      001026                        652 _mDelaymS:
      001026 AE 82            [24]  653 	mov	r6,dpl
      001028 AF 83            [24]  654 	mov	r7,dph
                                    655 ;	../include/debug.c:129: while ( n ) {
      00102A                        656 00101$:
      00102A EE               [12]  657 	mov	a,r6
      00102B 4F               [12]  658 	orl	a,r7
      00102C 60 15            [24]  659 	jz	00104$
                                    660 ;	../include/debug.c:134: mDelayuS( 1000 );
      00102E 90 03 E8         [24]  661 	mov	dptr,#0x03e8
      001031 C0 07            [24]  662 	push	ar7
      001033 C0 06            [24]  663 	push	ar6
      001035 12 10 10         [24]  664 	lcall	_mDelayuS
      001038 D0 06            [24]  665 	pop	ar6
      00103A D0 07            [24]  666 	pop	ar7
                                    667 ;	../include/debug.c:136: -- n;
      00103C 1E               [12]  668 	dec	r6
      00103D BE FF 01         [24]  669 	cjne	r6,#0xff,00116$
      001040 1F               [12]  670 	dec	r7
      001041                        671 00116$:
      001041 80 E7            [24]  672 	sjmp	00101$
      001043                        673 00104$:
                                    674 ;	../include/debug.c:138: }                                         
      001043 22               [24]  675 	ret
                                    676 ;------------------------------------------------------------
                                    677 ;Allocation info for local variables in function 'CH554UART0Alter'
                                    678 ;------------------------------------------------------------
                                    679 ;	../include/debug.c:147: void CH554UART0Alter()
                                    680 ;	-----------------------------------------
                                    681 ;	 function CH554UART0Alter
                                    682 ;	-----------------------------------------
      001044                        683 _CH554UART0Alter:
                                    684 ;	../include/debug.c:149: PIN_FUNC |= bUART0_PIN_X;                                                  //串口映射到P1.2和P1.3
      001044 AE C6            [24]  685 	mov	r6,_PIN_FUNC
      001046 43 06 10         [24]  686 	orl	ar6,#0x10
      001049 8E C6            [24]  687 	mov	_PIN_FUNC,r6
                                    688 ;	../include/debug.c:150: }
      00104B 22               [24]  689 	ret
                                    690 ;------------------------------------------------------------
                                    691 ;Allocation info for local variables in function 'mInitSTDIO'
                                    692 ;------------------------------------------------------------
                                    693 ;x                         Allocated with name '_mInitSTDIO_x_65536_17'
                                    694 ;x2                        Allocated with name '_mInitSTDIO_x2_65536_17'
                                    695 ;------------------------------------------------------------
                                    696 ;	../include/debug.c:161: void	mInitSTDIO( )
                                    697 ;	-----------------------------------------
                                    698 ;	 function mInitSTDIO
                                    699 ;	-----------------------------------------
      00104C                        700 _mInitSTDIO:
                                    701 ;	../include/debug.c:166: SM0 = 0;
                                    702 ;	assignBit
      00104C C2 9F            [12]  703 	clr	_SM0
                                    704 ;	../include/debug.c:167: SM1 = 1;
                                    705 ;	assignBit
      00104E D2 9E            [12]  706 	setb	_SM1
                                    707 ;	../include/debug.c:168: SM2 = 0;                                                                   //串口0使用模式1
                                    708 ;	assignBit
      001050 C2 9D            [12]  709 	clr	_SM2
                                    710 ;	../include/debug.c:170: RCLK = 0;                                                                  //UART0接收时钟
                                    711 ;	assignBit
      001052 C2 CD            [12]  712 	clr	_RCLK
                                    713 ;	../include/debug.c:171: TCLK = 0;                                                                  //UART0发送时钟
                                    714 ;	assignBit
      001054 C2 CC            [12]  715 	clr	_TCLK
                                    716 ;	../include/debug.c:172: PCON |= SMOD;
      001056 AE 87            [24]  717 	mov	r6,_PCON
      001058 43 06 80         [24]  718 	orl	ar6,#0x80
      00105B 8E 87            [24]  719 	mov	_PCON,r6
                                    720 ;	../include/debug.c:173: x = 10 * FREQ_SYS / UART0_BAUD / 16;                                       //如果更改主频，注意x的值不要溢出
      00105D 75 19 11         [24]  721 	mov	_mInitSTDIO_x_65536_17,#0x11
      001060 75 1A 04         [24]  722 	mov	(_mInitSTDIO_x_65536_17 + 1),#0x04
      001063 E4               [12]  723 	clr	a
      001064 F5 1B            [12]  724 	mov	(_mInitSTDIO_x_65536_17 + 2),a
      001066 F5 1C            [12]  725 	mov	(_mInitSTDIO_x_65536_17 + 3),a
                                    726 ;	../include/debug.c:174: x2 = x % 10;
      001068 75 51 0A         [24]  727 	mov	__modulong_PARM_2,#0x0a
      00106B F5 52            [12]  728 	mov	(__modulong_PARM_2 + 1),a
      00106D F5 53            [12]  729 	mov	(__modulong_PARM_2 + 2),a
      00106F F5 54            [12]  730 	mov	(__modulong_PARM_2 + 3),a
      001071 85 19 82         [24]  731 	mov	dpl,_mInitSTDIO_x_65536_17
      001074 85 1A 83         [24]  732 	mov	dph,(_mInitSTDIO_x_65536_17 + 1)
      001077 85 1B F0         [24]  733 	mov	b,(_mInitSTDIO_x_65536_17 + 2)
      00107A E5 1C            [12]  734 	mov	a,(_mInitSTDIO_x_65536_17 + 3)
      00107C 12 11 54         [24]  735 	lcall	__modulong
      00107F AC 82            [24]  736 	mov	r4,dpl
      001081 8C 1D            [24]  737 	mov	_mInitSTDIO_x2_65536_17,r4
                                    738 ;	../include/debug.c:175: x /= 10;
      001083 75 51 0A         [24]  739 	mov	__divulong_PARM_2,#0x0a
      001086 E4               [12]  740 	clr	a
      001087 F5 52            [12]  741 	mov	(__divulong_PARM_2 + 1),a
      001089 F5 53            [12]  742 	mov	(__divulong_PARM_2 + 2),a
      00108B F5 54            [12]  743 	mov	(__divulong_PARM_2 + 3),a
      00108D 85 19 82         [24]  744 	mov	dpl,_mInitSTDIO_x_65536_17
      001090 85 1A 83         [24]  745 	mov	dph,(_mInitSTDIO_x_65536_17 + 1)
      001093 85 1B F0         [24]  746 	mov	b,(_mInitSTDIO_x_65536_17 + 2)
      001096 E5 1C            [12]  747 	mov	a,(_mInitSTDIO_x_65536_17 + 3)
      001098 12 11 D7         [24]  748 	lcall	__divulong
      00109B 85 82 19         [24]  749 	mov	_mInitSTDIO_x_65536_17,dpl
      00109E 85 83 1A         [24]  750 	mov	(_mInitSTDIO_x_65536_17 + 1),dph
      0010A1 85 F0 1B         [24]  751 	mov	(_mInitSTDIO_x_65536_17 + 2),b
      0010A4 F5 1C            [12]  752 	mov	(_mInitSTDIO_x_65536_17 + 3),a
                                    753 ;	../include/debug.c:176: if ( x2 >= 5 ) x ++;                                                       //四舍五入
      0010A6 74 FB            [12]  754 	mov	a,#0x100 - 0x05
      0010A8 25 1D            [12]  755 	add	a,_mInitSTDIO_x2_65536_17
      0010AA 50 15            [24]  756 	jnc	00102$
      0010AC 74 01            [12]  757 	mov	a,#0x01
      0010AE 25 19            [12]  758 	add	a,_mInitSTDIO_x_65536_17
      0010B0 F5 19            [12]  759 	mov	_mInitSTDIO_x_65536_17,a
      0010B2 E4               [12]  760 	clr	a
      0010B3 35 1A            [12]  761 	addc	a,(_mInitSTDIO_x_65536_17 + 1)
      0010B5 F5 1A            [12]  762 	mov	(_mInitSTDIO_x_65536_17 + 1),a
      0010B7 E4               [12]  763 	clr	a
      0010B8 35 1B            [12]  764 	addc	a,(_mInitSTDIO_x_65536_17 + 2)
      0010BA F5 1B            [12]  765 	mov	(_mInitSTDIO_x_65536_17 + 2),a
      0010BC E4               [12]  766 	clr	a
      0010BD 35 1C            [12]  767 	addc	a,(_mInitSTDIO_x_65536_17 + 3)
      0010BF F5 1C            [12]  768 	mov	(_mInitSTDIO_x_65536_17 + 3),a
      0010C1                        769 00102$:
                                    770 ;	../include/debug.c:178: TMOD = TMOD & ~ bT1_GATE & ~ bT1_CT & ~ MASK_T1_MOD | bT1_M1;              //0X20，Timer1作为8位自动重载定时器
      0010C1 74 0F            [12]  771 	mov	a,#0x0f
      0010C3 55 89            [12]  772 	anl	a,_TMOD
      0010C5 FF               [12]  773 	mov	r7,a
      0010C6 43 07 20         [24]  774 	orl	ar7,#0x20
      0010C9 8F 89            [24]  775 	mov	_TMOD,r7
                                    776 ;	../include/debug.c:179: T2MOD = T2MOD | bTMR_CLK | bT1_CLK;                                        //Timer1时钟选择
      0010CB 43 C9 A0         [24]  777 	orl	_T2MOD,#0xa0
                                    778 ;	../include/debug.c:180: TH1 = 0-x;                                                                 //12MHz晶振,buad/12为实际需设置波特率
      0010CE AF 19            [24]  779 	mov	r7,_mInitSTDIO_x_65536_17
      0010D0 C3               [12]  780 	clr	c
      0010D1 E4               [12]  781 	clr	a
      0010D2 9F               [12]  782 	subb	a,r7
      0010D3 F5 8D            [12]  783 	mov	_TH1,a
                                    784 ;	../include/debug.c:181: TR1 = 1;                                                                   //启动定时器1
                                    785 ;	assignBit
      0010D5 D2 8E            [12]  786 	setb	_TR1
                                    787 ;	../include/debug.c:182: TI = 1;
                                    788 ;	assignBit
      0010D7 D2 99            [12]  789 	setb	_TI
                                    790 ;	../include/debug.c:183: REN = 1;                                                                   //串口0接收使能
                                    791 ;	assignBit
      0010D9 D2 9C            [12]  792 	setb	_REN
                                    793 ;	../include/debug.c:184: }
      0010DB 22               [24]  794 	ret
                                    795 ;------------------------------------------------------------
                                    796 ;Allocation info for local variables in function 'CH554UART0RcvByte'
                                    797 ;------------------------------------------------------------
                                    798 ;	../include/debug.c:193: uint8_t  CH554UART0RcvByte( )
                                    799 ;	-----------------------------------------
                                    800 ;	 function CH554UART0RcvByte
                                    801 ;	-----------------------------------------
      0010DC                        802 _CH554UART0RcvByte:
                                    803 ;	../include/debug.c:195: while(RI == 0);                                                            //查询接收，中断方式可不用
      0010DC                        804 00101$:
                                    805 ;	../include/debug.c:196: RI = 0;
                                    806 ;	assignBit
      0010DC 10 98 02         [24]  807 	jbc	_RI,00114$
      0010DF 80 FB            [24]  808 	sjmp	00101$
      0010E1                        809 00114$:
                                    810 ;	../include/debug.c:197: return SBUF;
      0010E1 85 99 82         [24]  811 	mov	dpl,_SBUF
                                    812 ;	../include/debug.c:198: }
      0010E4 22               [24]  813 	ret
                                    814 ;------------------------------------------------------------
                                    815 ;Allocation info for local variables in function 'CH554UART0SendByte'
                                    816 ;------------------------------------------------------------
                                    817 ;SendDat                   Allocated to registers 
                                    818 ;------------------------------------------------------------
                                    819 ;	../include/debug.c:207: void CH554UART0SendByte(uint8_t SendDat)
                                    820 ;	-----------------------------------------
                                    821 ;	 function CH554UART0SendByte
                                    822 ;	-----------------------------------------
      0010E5                        823 _CH554UART0SendByte:
      0010E5 85 82 99         [24]  824 	mov	_SBUF,dpl
                                    825 ;	../include/debug.c:210: while(TI ==0);
      0010E8                        826 00101$:
                                    827 ;	../include/debug.c:211: TI = 0;
                                    828 ;	assignBit
      0010E8 10 99 02         [24]  829 	jbc	_TI,00114$
      0010EB 80 FB            [24]  830 	sjmp	00101$
      0010ED                        831 00114$:
                                    832 ;	../include/debug.c:212: }
      0010ED 22               [24]  833 	ret
                                    834 ;------------------------------------------------------------
                                    835 ;Allocation info for local variables in function 'putchar'
                                    836 ;------------------------------------------------------------
                                    837 ;c                         Allocated to registers r6 r7 
                                    838 ;------------------------------------------------------------
                                    839 ;	../include/debug.c:229: int putchar(int c)
                                    840 ;	-----------------------------------------
                                    841 ;	 function putchar
                                    842 ;	-----------------------------------------
      0010EE                        843 _putchar:
      0010EE AE 82            [24]  844 	mov	r6,dpl
      0010F0 AF 83            [24]  845 	mov	r7,dph
                                    846 ;	../include/debug.c:231: while (!TI) /* assumes UART is initialized */
      0010F2                        847 00101$:
                                    848 ;	../include/debug.c:233: TI = 0;
                                    849 ;	assignBit
      0010F2 10 99 02         [24]  850 	jbc	_TI,00114$
      0010F5 80 FB            [24]  851 	sjmp	00101$
      0010F7                        852 00114$:
                                    853 ;	../include/debug.c:234: SBUF = c & 0xFF;
      0010F7 8E 99            [24]  854 	mov	_SBUF,r6
                                    855 ;	../include/debug.c:236: return c;
      0010F9 8E 82            [24]  856 	mov	dpl,r6
      0010FB 8F 83            [24]  857 	mov	dph,r7
                                    858 ;	../include/debug.c:237: }
      0010FD 22               [24]  859 	ret
                                    860 ;------------------------------------------------------------
                                    861 ;Allocation info for local variables in function 'getchar'
                                    862 ;------------------------------------------------------------
                                    863 ;	../include/debug.c:239: int getchar() {
                                    864 ;	-----------------------------------------
                                    865 ;	 function getchar
                                    866 ;	-----------------------------------------
      0010FE                        867 _getchar:
                                    868 ;	../include/debug.c:240: while(!RI); /* assumes UART is initialized */
      0010FE                        869 00101$:
                                    870 ;	../include/debug.c:241: RI = 0;
                                    871 ;	assignBit
      0010FE 10 98 02         [24]  872 	jbc	_RI,00114$
      001101 80 FB            [24]  873 	sjmp	00101$
      001103                        874 00114$:
                                    875 ;	../include/debug.c:242: return SBUF;
      001103 AE 99            [24]  876 	mov	r6,_SBUF
      001105 7F 00            [12]  877 	mov	r7,#0x00
      001107 8E 82            [24]  878 	mov	dpl,r6
      001109 8F 83            [24]  879 	mov	dph,r7
                                    880 ;	../include/debug.c:243: }
      00110B 22               [24]  881 	ret
                                    882 ;------------------------------------------------------------
                                    883 ;Allocation info for local variables in function 'CH554UART1Alter'
                                    884 ;------------------------------------------------------------
                                    885 ;	../include/debug.c:253: void CH554UART1Alter()
                                    886 ;	-----------------------------------------
                                    887 ;	 function CH554UART1Alter
                                    888 ;	-----------------------------------------
      00110C                        889 _CH554UART1Alter:
                                    890 ;	../include/debug.c:255: PIN_FUNC |= bUART1_PIN_X;
      00110C AE C6            [24]  891 	mov	r6,_PIN_FUNC
      00110E 43 06 20         [24]  892 	orl	ar6,#0x20
      001111 8E C6            [24]  893 	mov	_PIN_FUNC,r6
                                    894 ;	../include/debug.c:256: }
      001113 22               [24]  895 	ret
                                    896 ;------------------------------------------------------------
                                    897 ;Allocation info for local variables in function 'UART1Setup'
                                    898 ;------------------------------------------------------------
                                    899 ;	../include/debug.c:265: void	UART1Setup( )
                                    900 ;	-----------------------------------------
                                    901 ;	 function UART1Setup
                                    902 ;	-----------------------------------------
      001114                        903 _UART1Setup:
                                    904 ;	../include/debug.c:267: U1SM0 = 0;                                                                   //UART1选择8位数据位
                                    905 ;	assignBit
      001114 C2 C7            [12]  906 	clr	_U1SM0
                                    907 ;	../include/debug.c:268: U1SMOD = 1;                                                                  //快速模式
                                    908 ;	assignBit
      001116 D2 C5            [12]  909 	setb	_U1SMOD
                                    910 ;	../include/debug.c:269: U1REN = 1;                                                                   //使能接收
                                    911 ;	assignBit
      001118 D2 C4            [12]  912 	setb	_U1REN
                                    913 ;	../include/debug.c:270: SBAUD1 = 256 - FREQ_SYS/16/UART1_BAUD;
      00111A 75 C2 98         [24]  914 	mov	_SBAUD1,#0x98
                                    915 ;	../include/debug.c:271: }
      00111D 22               [24]  916 	ret
                                    917 ;------------------------------------------------------------
                                    918 ;Allocation info for local variables in function 'CH554UART1RcvByte'
                                    919 ;------------------------------------------------------------
                                    920 ;	../include/debug.c:280: uint8_t  CH554UART1RcvByte( )
                                    921 ;	-----------------------------------------
                                    922 ;	 function CH554UART1RcvByte
                                    923 ;	-----------------------------------------
      00111E                        924 _CH554UART1RcvByte:
                                    925 ;	../include/debug.c:282: while(U1RI == 0);                                                           //查询接收，中断方式可不用
      00111E                        926 00101$:
                                    927 ;	../include/debug.c:283: U1RI = 0;
                                    928 ;	assignBit
      00111E 10 C0 02         [24]  929 	jbc	_U1RI,00114$
      001121 80 FB            [24]  930 	sjmp	00101$
      001123                        931 00114$:
                                    932 ;	../include/debug.c:284: return SBUF1;
      001123 85 C1 82         [24]  933 	mov	dpl,_SBUF1
                                    934 ;	../include/debug.c:285: }
      001126 22               [24]  935 	ret
                                    936 ;------------------------------------------------------------
                                    937 ;Allocation info for local variables in function 'CH554UART1SendByte'
                                    938 ;------------------------------------------------------------
                                    939 ;SendDat                   Allocated to registers 
                                    940 ;------------------------------------------------------------
                                    941 ;	../include/debug.c:294: void CH554UART1SendByte(uint8_t SendDat)
                                    942 ;	-----------------------------------------
                                    943 ;	 function CH554UART1SendByte
                                    944 ;	-----------------------------------------
      001127                        945 _CH554UART1SendByte:
      001127 85 82 C1         [24]  946 	mov	_SBUF1,dpl
                                    947 ;	../include/debug.c:297: while(U1TI ==0);
      00112A                        948 00101$:
                                    949 ;	../include/debug.c:298: U1TI = 0;
                                    950 ;	assignBit
      00112A 10 C1 02         [24]  951 	jbc	_U1TI,00114$
      00112D 80 FB            [24]  952 	sjmp	00101$
      00112F                        953 00114$:
                                    954 ;	../include/debug.c:299: }
      00112F 22               [24]  955 	ret
                                    956 ;------------------------------------------------------------
                                    957 ;Allocation info for local variables in function 'CH554WDTModeSelect'
                                    958 ;------------------------------------------------------------
                                    959 ;mode                      Allocated to registers r7 
                                    960 ;------------------------------------------------------------
                                    961 ;	../include/debug.c:310: void CH554WDTModeSelect(uint8_t mode)
                                    962 ;	-----------------------------------------
                                    963 ;	 function CH554WDTModeSelect
                                    964 ;	-----------------------------------------
      001130                        965 _CH554WDTModeSelect:
      001130 AF 82            [24]  966 	mov	r7,dpl
                                    967 ;	../include/debug.c:312: SAFE_MOD = 0x55;
      001132 75 A1 55         [24]  968 	mov	_SAFE_MOD,#0x55
                                    969 ;	../include/debug.c:313: SAFE_MOD = 0xaa;                                                             //进入安全模式
      001135 75 A1 AA         [24]  970 	mov	_SAFE_MOD,#0xaa
                                    971 ;	../include/debug.c:314: if(mode){
      001138 EF               [12]  972 	mov	a,r7
      001139 60 0B            [24]  973 	jz	00102$
                                    974 ;	../include/debug.c:315: GLOBAL_CFG |= bWDOG_EN;                                                    //启动看门狗复位
      00113B AE B1            [24]  975 	mov	r6,_GLOBAL_CFG
      00113D 7F 00            [12]  976 	mov	r7,#0x00
      00113F 43 06 01         [24]  977 	orl	ar6,#0x01
      001142 8E B1            [24]  978 	mov	_GLOBAL_CFG,r6
      001144 80 03            [24]  979 	sjmp	00103$
      001146                        980 00102$:
                                    981 ;	../include/debug.c:317: else GLOBAL_CFG &= ~bWDOG_EN;	                                            //启动看门狗仅仅作为定时器
      001146 53 B1 FE         [24]  982 	anl	_GLOBAL_CFG,#0xfe
      001149                        983 00103$:
                                    984 ;	../include/debug.c:318: SAFE_MOD = 0x00;                                                             //退出安全模式
      001149 75 A1 00         [24]  985 	mov	_SAFE_MOD,#0x00
                                    986 ;	../include/debug.c:319: WDOG_COUNT = 0;                                                              //看门狗赋初值
      00114C 75 FF 00         [24]  987 	mov	_WDOG_COUNT,#0x00
                                    988 ;	../include/debug.c:320: }
      00114F 22               [24]  989 	ret
                                    990 ;------------------------------------------------------------
                                    991 ;Allocation info for local variables in function 'CH554WDTFeed'
                                    992 ;------------------------------------------------------------
                                    993 ;tim                       Allocated to registers 
                                    994 ;------------------------------------------------------------
                                    995 ;	../include/debug.c:331: void CH554WDTFeed(uint8_t tim)
                                    996 ;	-----------------------------------------
                                    997 ;	 function CH554WDTFeed
                                    998 ;	-----------------------------------------
      001150                        999 _CH554WDTFeed:
      001150 85 82 FF         [24] 1000 	mov	_WDOG_COUNT,dpl
                                   1001 ;	../include/debug.c:333: WDOG_COUNT = tim;                                                             //看门狗计数器赋值
                                   1002 ;	../include/debug.c:334: }
      001153 22               [24] 1003 	ret
                                   1004 	.area CSEG    (CODE)
                                   1005 	.area CONST   (CODE)
                                   1006 	.area XINIT   (CODE)
                                   1007 	.area CABS    (ABS,CODE)
