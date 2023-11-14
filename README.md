# Swift

## Installation
- OSX is an operating system made by Apple for Mac computers.
- Need OSX to run iOS apps.
 
PC:

- If you have a PC, you need to use a process called virtualisation: running an operating system on your computer. You will need the following:
	- VMware Player allows you to create a virtual machine on your computer, to run a different operating system on windows machine.
	- need Microsoft Hardware-Assisted Virtualisation Detection Tool, which will tell you if your computer is compatible and able to run what is needed. 
	- WinRAR will allow you to extract some of the software you download. 
	- Need a copy of OSX itself. 

Mac:

- Xcode: complete piece of software that allows you to design, code, and submit an app. 

## Xcode
- Let's take a look at Xcode and how it works. Let's also work with the **storyboard**. 
- Let's discuss **Auto Layout**. 

## Swift

- New language announced in June 2014. 
- Playgrounds allow you to run code immediately and see the results. 
- Let's go over what you will see at the beginning of your code base and what it means:

	- `import UIkit` imports a range of functions and methods that allow you to interact with the user interface.
	- This will be followed by this:

	```
	class ViewController: UIViewController {

	    override func viewDidLoad() {
	        super.viewDidLoad()
	        // Do any additional setup after loading the view, typically from a nib.
	    }

	    override func didReceiveMemoryWarning() {
	        super.didReceiveMemoryWarning()
	        // Dispose of any resources that can be recreated.
	    }


	}

	```
- `println("Hello World!")` allows you to print simple code in your log(the console). Why would we want to do this?  

- `var` creates a variable, when you want to set it equal to a value you place it in quotes. 
- `variable` = bucket or store for a particular value.
- Swift is very sensitive to types of variables. 
- To update a variable:
	
	```
	var str = "Hello"
	
	str = "Goodbye" 
	
	```
	
- To specify that a variable is a **string**(a collection of characters):
	
	`var name:String = "Mel"`
	
- **Integers** are whole numbers (example: used if you are counting the number of users in your database).
	
	```
	var int = 4
	
	4 * int
	
	```
	- To specify that a variable is an integer:
	
	 `var a:Int = 5`
	
- **Double** specifies that the number is a decimal:
	
	 `var c:Double = 3 / 2`
	
- Can't combine integers and doubles, need to convert integer in to a double: `c*Double(int)`
	
- **Three core variables: strings, integers, doubles.**

	`var longSentence = str + name`
	
- **Array** is a collection of variables (example: you want to store all of the user's posts, can then loop through them and search for a particular one).

	`var arr = [1, 2, 3]`
	
	- If you wanted to access the 3rd variable:
	
		`arr[2]`
	
	- To add an item to an array:
	
		`arr.append(4)`
	
- An array is ordered, a **dictionary** is not.

	`var dict = ["name": "Mel", "age": 28, "gender": "female"]`
	
	`println(dict["name"])`
	
- **Generics** allows you to write flexible, reusable functions and types that can work with any type, subject to requirements that you define. You can write code that avoids duplication and expresses its intent in a clear manner. `Array` and `Dictionary` types are both generic collections. 
	
- An **optional** is a variable that may or may not have a value.

	- To specify that the variable has a value, you can do the following: `println(dict["name"]!)`

-----------------------------------Practice Time----------------------------------------

- **Initialization** is the process of preparing an instance of a class, structure, or enumeration for use. This process involves setting an initial value for each stored property on that instance and performing any other setup that is required before the new instance is ready for use.

	```
	struct Fahrenheit {
	    var temperature: Double
	    init() {
	        temperature = 32.0
	    }
	}
	var f = Fahrenheit()
	println("The default temperature is \(f.temperature)° Fahrenheit")
	// prints "The default temperature is 32.0° Fahrenheit"
		
	```
	
- **Closures** are self-contained blocks of functionality that can be passed around and used in your code. Closures can capture and store references to any constants and variables from the context in which they are defined. This is known as closing over those constants and variables. Swift handles all of the memory management of capturing for you.
	
	
	
	
	
