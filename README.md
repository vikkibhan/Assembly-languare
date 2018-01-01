# Assembly-language
;to print the string

section .data
				msg	db	'hey, i am github'
				msglen equ	$-msg
				
section .text
				global _start:
_start:
				mov			eax,4
				mov			ebx,1
				mov			ecx,msg
				mov			edx,msglen
				int			80H
				
				mov			eax,1
				mov			ebx,0
				int			80H

      
