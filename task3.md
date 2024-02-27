By Referring to C-based Lab videos and RISC-V-based lab videos

Snapshots of the compiled C code and RISC-V

Step 1: check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) If the leafpad editor is opened without any errors then type the C code. **If the leafpad is not installed in ur machine then install by using the following command

sudo snap install leafpad**
![Screenshot 2024-02-27 162208](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/ef772197-97c6-43e6-a64e-5d5adb8fcc2b)

**Step 2: Writing the C code in the leafpad editor using the following command

leafpad sum1ton.c&

![2nd p](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/5058836f-e55c-4ac3-9a64-3ed5a3e43ef9)

Step 3: After writing the C code save the editor by Ctrl+s

Step 4: Check for the errors by using the following command(compilation step)

gcc sum1ton.c
./a.out
Sum of numbers from 1 to 500 is 125250


![Screenshot 2024-02-27 162307](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/142baf51-11e9-4227-91e5-dcc69bfb743a)
***RISCV Compilation and Execution

Step 1: View the C Code in the editor window using the following command

cat sum1ton.c
![Screenshot 2024-02-27 162456](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/f21441bb-1c0e-4e87-9abc-b65fafbb3d31)

Step 2: Compile the code in riscv using the following command

riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
![Screenshot 2024-02-27 162524](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/6d3cc6e8-6003-406b-9bfa-a55bb2d3e457)

Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.

use the command
ls -ltr sum1ton.c
![Screenshot 2024-02-27 162550](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/7ff075de-ba8f-463e-aa49-cc19c038e727)


![Screenshot 2024-02-27 162617](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/38f054ee-0501-4c53-8866-d715555b7c8d)



![Screenshot 2024-02-27 162647](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/0516d5e3-0006-493b-b0ce-861e65125dc1)
Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution

![Screenshot 2024-02-27 162708](https://github.com/anushreepatilgithub/VSDSQUADRON-MINI/assets/160833293/e7add478-2b07-434e-a6fd-249fc2663ca3)
