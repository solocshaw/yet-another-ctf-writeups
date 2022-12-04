### Challenge Description

*No description*

Author: 0xRF

Attachments:
- [sanity-check](attachments/sanity-check/sanity-check)

### Solution 

We can run the `strings` command on the above file to get the following output:

```
/lib64/ld-linux-x86-64.so.2
libc.so.6
strncpy
__stack_chk_fail
strlen
memcpy
__cxa_finalize
__libc_start_main
GLIBC_2.14
GLIBC_2.4
GLIBC_2.2.5
_ITM_deregisterTMCloneTable
__gmon_start__
_ITM_registerTMCloneTable
u+UH
|M_$0RR
Y_|_L37
_Y0U_D0
[]A\A]A^A_
UACTF{N3V3R_G0NN4_L37_Y0U_D0WN}
:*3$"
GCC: (Ubuntu 9.3.0-17ubuntu1~20.04) 9.3.0
crtstuff.c
deregister_tm_clones
__do_global_dtors_aux
completed.8060
__do_global_dtors_aux_fini_array_entry
frame_dummy
__frame_dummy_init_array_entry
main.c
flag
__FRAME_END__
__init_array_end
_DYNAMIC
__init_array_start
__GNU_EH_FRAME_HDR
_GLOBAL_OFFSET_TABLE_
__libc_csu_fini
strncpy@@GLIBC_2.2.5
_ITM_deregisterTMCloneTable
_edata
strlen@@GLIBC_2.2.5
__stack_chk_fail@@GLIBC_2.4
__libc_start_main@@GLIBC_2.2.5
__data_start
__gmon_start__
__dso_handle
memcpy@@GLIBC_2.14
_IO_stdin_used
__libc_csu_init
__bss_start
main
__TMC_END__
_ITM_registerTMCloneTable
do_stuff
__cxa_finalize@@GLIBC_2.2.5
.symtab
.strtab
.shstrtab
.interp
.note.gnu.property
.note.gnu.build-id
.note.ABI-tag
.gnu.hash
.dynsym
.dynstr
.gnu.version
.gnu.version_r
.rela.dyn
.rela.plt
.init
.plt.got
.plt.sec
.text
.fini
.rodata
.eh_frame_hdr
.eh_frame
.init_array
.fini_array
.dynamic
.data
.bss
.comment

```

<details>
  <summary>Click to see flag</summary> 
  
    UACTF{N3V3R_G0NN4_L37_Y0U_D0WN}

</details>