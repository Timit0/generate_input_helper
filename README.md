# generate_input_helper
generate_input_helper is a simple tool written in c++.

## Why should I use this tool instead of using strings
If you want change an input name.

<details>
  <summary>String</summary>
  
  You have to change everywhere in your project this can be long and some can be forgotten therefore creating
errors
</details>

<details>
  <summary>Tool</summary>
  
  Just rename your variable and it will change everywhere
</details>


If you have many input.

<details>
  <summary>String</summary>
  
  This can be very long like several hours in extreme case.
</details>

<details>
  <summary>Tool</summary>
  
  Less than 2 minutes and 1 of these 2 minutes is for reading the tuto
</details>


## Tutorial

### context
Exe location - ```C:\My\Custom\Path\helper.exe```

Godot project file location - ```C:\My\Other\Custom\Location\project.godot```

I have set 3 custom input in godot
- custom1
- custom2
- custom3

### Tuto
In cmd at exe location 

\> ```helper.exe```

The program ask you "Enter project.godot path : "

\> ```C:\My\Other\Custom\Location\project.godot```

The program ask you "Enter the output path : "

\> ```C:\A\Location\I\Have\Decided\```

The program ask you "Set the file and class name" no space or special character

\> ```MyInputs```

The result will be

```
public static class MyInputs
{
    public static string custom1
	{
		get
		{
			return nameof(custom1);
		}
	}
	public static string custom2
	{
		get
		{
			return nameof(custom2);
		}
	}
	public static string custom3
	{
		get
		{
			return nameof(custom3);
		}
	}
}
```
