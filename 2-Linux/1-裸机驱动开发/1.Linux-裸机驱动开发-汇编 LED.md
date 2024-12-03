# Linux-裸机驱动开发-汇编 LED

## 软件编写

```assembly
.global _start

-start:
	LDR R0, =0x020C4068
	LDR R1, =0xFFFFFFFF
	STR R1, [R0]
	
	LDR R0, =0x020C406C
	LDR R1, =0xFFFFFFFF
	STR R1, [R0]
	
	LDR R0, =0x020C4070
	LDR R1, =0xFFFFFFFF
	STR R1, [R0]
	
    LDR R0, =0x020C4074
	LDR R1, =0xFFFFFFFF
	STR R1, [R0]
	
	LDR R0, =0x020C4078
	LDR R1, =0xFFFFFFFF
	STR R1, [R0]
	
	LDR R0, =0x020C407C
	LDR R1, =0xFFFFFFFF
	STR R1, [R0]
	
	LDR R0, =0x020C4080
	LDR R1, =0xFFFFFFFF
	STR R1, [R0]
```

