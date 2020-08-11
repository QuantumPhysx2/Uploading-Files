# Uploading-Files
.NET Core 3

This method of uploading a file only focuses on uploading a SINGLE file. NOT multiple, nor displaying multiple.

Additionally, input validation and other security practices are not focused on here (deliberately).

Reference:
https://csharp-video-tutorials.blogspot.com/2019/05/file-upload-in-aspnet-core-mvc.html


<br />
<h1>Logic behind image uploading</h1>
<code>
  // .NET Core C# - Uploading an Image Function

// Important to set as an 'Asynchronous' function
public async Task<IActionResult> Create(<Model Binding stuff so that we add data to model on POST>, <Create a reference to our target Model>) 
{
	if (ModelState.IsValid)
	{
		// define our wwwroot path
		// setup a Guid instance
		// define our filename without the extension
		// define our extension from the input file
		// append our Guid instance + filename + current datetime + extension
		// combine our 'wwwroot' path with '/images/'
		// combine our 'wwwroot/images/' path with our input file (filename)
		// begin using statement -> a var which instantiates a new FileStream session >>> pass in our 'wwwroot/images/<input_file>' and set in 'Create' mode
		// reference our Model's respective 'Image' column and add it by copying the filestream variable to our model
		// save the record
	}
}
</code>
