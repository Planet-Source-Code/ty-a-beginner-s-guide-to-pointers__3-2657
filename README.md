<div align="center">

## A Beginner's Guide to Pointers


</div>

### Description

An Example on the Usage of Pointers
 
### More Info
 
Always be careful to know the exact location in memory pointers are aiming at before changing the values they point to.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Ty](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/ty.md)
**Level**          |Beginner
**User Rating**    |4.3 (34 globes from 8 users)
**Compatibility**  |C, C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__3-32.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/ty-a-beginner-s-guide-to-pointers__3-2657/archive/master.zip)





### Source Code

```
//Free Source Code Tutorials Free for the taking
//Blazon Resources
//http://www.members.home.net/blazonres
//
//Email at blazonres@home.com
#include <iostream.h>
void main()
{
	int MemoryAddress = 0;	//Value in memory to point to
	int *Pointer;			//Stores(Points to) value of memory location
	Pointer = &MemoryAddress;	//Point to the address of 'MemoryAddress'
	//No '*' used here because it points to the location of 'MemoryAddress'
	//Pointer now knows where the value of 'MemoryAddress' is and
	//therefore can be used to change it (as used here from 0 to 1)
	cout << MemoryAddress << endl;	//Show the value of 'MemoryAddress'
	*Pointer = 1;	//Point to the location in memory and change the value to 1
	cout << MemoryAddress << endl;	//Show the new value of 'MemoryAddress' on the screen
}
/*
NOTE:
Changing the value of an unknown memory location may cause the computer
to crash or lose vital information causing serious problems.
Ommitting the line:
"Pointer = &MemoryAddress;"
will cause the program to change a nearly random location in memory which
could cause serious damage to the computer. So be sure to define the location
in memory that is intended to be changed
*/
```

