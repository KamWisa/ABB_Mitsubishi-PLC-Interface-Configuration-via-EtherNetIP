RJ71EIP91 สามารถเชื่อมกับ 1 -64
ค่า K ด้านหน้าคือ Station K1 - K64

M_RJ71EIP91_Class1GetInputData_00A
Input 
i_bEN                  Bit	                                VAR_INPUT	0	          Execution command
i_stModule	           M+RJ71EIP91	                        VAR_INPUT		          Module label
i_uConnectionNo	       Word [Unsigned]/Bit String [16-bit]	VAR_INPUT	0	          Connection Number
SM400 เชื่อมต่อ
EIP91_1 
Station [ K1 - K64 ]

Output
o_bENO	        Bit	                                VAR_OUTPUT	0	Execution status
o_bOK	          Bit	                                VAR_OUTPUT	0	Normal completion
o_bEｒｒ	      Bit	                                VAR_OUTPUT	0	Error completion
o_uErrId	      Word [Unsigned]/Bit String [16-bit]	VAR_OUTPUT	0	Error code
o_uStatusId	    Word [Unsigned]/Bit String [16-bit]	VAR_OUTPUT	0	Error code of connection communication error
o_uInputData	  Word [Unsigned]/Bit String [16-bit]	VAR_OUTPUT	0	Input data storage device

o_uInputData = ใส่ Data Output Start [ D xxx ]

-------------------------------------

M_RJ71EIP91_Class1SetOutputData_00A
Input
i_bEN	                Bit	                                VAR_INPUT	0	Execution command
i_stModule	          M+RJ71EIP91	                        VAR_INPUT		Module label
i_uConnectionNo	      Word [Unsigned]/Bit String [16-bit]	VAR_INPUT	0	Connection Number
i_uOutputData	        Word [Unsigned]/Bit String [16-bit]	VAR_INPUT	0	Output data storage device

i_stModule = EIP91_1
i_uConnectionNo = Station [ K1 - K64 ]
i_uOutputData = ใส่ Data Output Start [ D xxx ]
