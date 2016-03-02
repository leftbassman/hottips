# Hot Tips

In development, utilizing shortcuts and organizational practices can take your productivity to the next level. This list is a collection of tips and tricks that are important to follow to keep your process free of confusion.!

## Terminology

- **Operating System** - The visual interface you see on your computer. This is often known as 'Windows' or 'Mac OSX' depending on your computer.
- **Finder/Explorer** - A visual representation of the files and folders on your computer. On Windows, it is called 'Windows Explorer", on Mac it is called 'Finder'.
- **File path** - A path to a file or folder on a computer. Used to reference one file with another.
- **Local** - Code, a file or a website that is stored/located on our physical computers.
- **Remote** - Code, a file or a website that is stored/located elsewhere on the internet.
- **Root** - The lowest point of a project folder or a file directory.

## File Paths

Within HackerYou content, lessons and in online third-party tutorials, you're going to see some common syntax to represent file structure.

For this bit, take the following folder structure: 

```text
- myProject
	- images
		- dog.jpg
		- cat.jpg
	- styles
		- main.css
	- index.html
```

We have a folder named 'myProject' that contains one single file and two folders. The single file is `index.html` and the two folders are `images` and `styles`.

The `images` folder contains two files, `dog.jpg` and `cat.jpg`.

The `styles` folder contains one file, `main.css`.

### Referencing an internal file

To reference an image, we could write the following file path that starts at the root of our folder (`myProject`), which shows the full path to the file through the folder system.

```
images/dog.jpg
```

This is how we can import files into other files, we reference the relative path. If we are using the `index.html` file, we can reference an image by creating a path to it through the project structure.

**index.html**
```html
<img src="images/cat.jpg" alt="A cool cat!" />
```

### Going back a folder
Using our above folder structure, what happens if we need to refer to a file in a folder that's not accessible in a linear direction like above?

For this example, we'll assume that we're in the `main.css` file that is located in the `styles` folder, and we want to reference our `dog.jpg` file again.

If we were to simply type `images/dog.jpg`, we would be saying that we want a folder that's in the same directory as the `main.css`, and that contains `dog.jpg`.

```css
.item {
	background: url(images/dog.jpg);
}
```

In fact, we need to move back a folder, into the root of the project, and then into the images folder. To accomplish this, we use `../` to say __'go back a folder'__.

```css
.item {
	background: url(../images/dog.jpg);
}
```


## File + Folder Organization

1. Keep files off your desktop, you should have a ~/Sites or a ~/Dropbox/sites folder to all your projects

1. Folders should be all lowercase without spaces. 
  
	  **BAD:**
	  
	  Hacker You Project 1

	  CSS Testing
	  
	  ------project 2 -------

	  **Good:**
	  
	  hackeryou_project_1
	  
	  css_testing
	  
	  project-2


# Must Know shortcuts

Learn These Shortcuts. Don't use your mouse when you don't have to:

`⌘` + `Tab` to switch between applications. Keep holding down `⌘` and use your arrow keys to move to another application.

`⌘` + `~` to switch between multiple windows of an app (Like Sublime Text)

`⌘` + `⌥` (option) + `←/→` move between tabs of _any_ application

`⌘` + `1-8` to select specific tabs (left to right order) of _any_ application

`⌘` + `9` to select the last tab of _most_ applications

`⌘` + `T` to create a new tab

`⌘` + `W` to close the Current Tab

`⌘` + `Shift` + `T` to open the last closed tab

`⌘` + `S` to Save

`⌘` + `Shift` + `S` to Save a new file

`⌘` + `Shift` + `←/→` to highlight whole lines of text

`⌥` + `←/→` to move your cursor word-by-word

`⌥` + `Shift` + `←/→` to select text word-by-word 

`⌘` + `C` to Copy

`⌘` + `V` to Paste

`⌘` + `X` to Cut

`⌘` + `Z` to Undo

`⌘` + `Shift` + `Z` to Redo
