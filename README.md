# Report for Assignment 1

## Project chosen

Name: Pyinstaller

URL: https://github.com/EssamFattah/pyinstaller.git

Number of lines of code and the tool used to count it: 60,825 TOTAL, 42,000 written in Python (used lizard to count)

Programming language: Python

## Coverage measurement

### Existing tool

After downloading the necessary modules from the requirements.txt file using “pip install -r requirements.txt”, we used the Coverage.py command  “coverage run --source=. -m pytest” to test the coverage of our code. We then translated the results into HTML to help us better visualise the coverage using “coverage html”:

<img width="791" alt="1" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/91b60355-69a6-43b6-b7d3-ee1e60f4bda5">

We find a coverage of 60 percent for the project.

### Your own coverage tool

Future (Essam) Abdel Fattah:

Function 1 name: build_script(text_options=None, always_on_top=False)

Commit link: https://github.com/pyinstaller/pyinstaller/commit/b0aacbd4fd1e696b1157b3e74dad9238b00b7b10#



Function 2 name:  _module_collection_mode_sanitizer(value)


Commit link:
https://github.com/pyinstaller/pyinstaller/commit/9e222041cd34a99393c73905675d422f3ea1b8dc

Member 2 Seleem Wagdy:

Function 1 name: make_path_spec_relative(filename, spec_dir)

Commit link:
https://github.com/pyinstaller/pyinstaller/commit/664f977348b4e57cd3422dc6b985e3b82cdd4657

	Function 2 name:  _check_guts_eq(attr_name, old_value, new_value, last_build)
Commit link:
https://github.com/pyinstaller/pyinstaller/commit/fb1013de80eadff211f11ac69d2f5e3aa280b621

## Coverage improvement

### Individual tests

Member 1 Future (Essam) Abdel Fattah:
Test 1:

Commit: https://github.com/pyinstaller/pyinstaller/commit/b0aacbd4fd1e696b1157b3e74dad9238b00b7b10#

Old coverage results:


New coverage results:



We created a test case where the font is “TKDefault” as well as a test case where the font is “Helvetica”, this made sure that the code in the conditional statements is covered. We can see this is the case because of the green highlight seen in the screenshot above.



Test 2:

Old coverage results:


New coverage results:


We created 2 test cases to cover both of the branches seen in the code, the first test case tests when value is a dictionary variable, and the second test case tests when value is a string variable. This properly covers both available branches of the function.

Commit link:
https://github.com/pyinstaller/pyinstaller/commit/9e222041cd34a99393c73905675d422f3ea1b8dc


Member 2: Seleem Wagdy

Test 1:
<Show a patch (diff) or a link to a commit made in your forked repository that shows the new/enhanced test>

	Old coverage:
	
	
	New coverage:
	

For this function, we created two test cases that would cover the available branches. The first case takes filename to be an absolute path (“//”), while the second test case takes to be a normal path (“C:”).


Commit link:
https://github.com/pyinstaller/pyinstaller/commit/664f977348b4e57cd3422dc6b985e3b82cdd4657

Task 2:
<Show a patch (diff) or a link to a commit made in your forked repository that shows the new/enhanced test>

Old coverage: 

New coverage:

We created two test cases to cover both branches present in this function, first we created a test cases where old_value and new_value are different, and a test case where they are the same.


Commit link:
https://github.com/pyinstaller/pyinstaller/commit/fb1013de80eadff211f11ac69d2f5e3aa280b621

### Overall

Old coverage:


New coverage:


We can see a coverage increase of 1% on the overall code, down below you can see the individual files that were modified, and how their coverage was affected after our tests were implemented.

Splash_templates before:

Splash_templates after:


Imphook before:

Imphook after:

utils before:

Utils after:


Makespec before:

Makespec after:


## Statement of individual contributions
Looked for a suitable repository: Future and Seleem
Figured out how to run the coverage test: Future and Seleem
Took care of the forked repository: Future
Wrote and put together the documentation: Seleem
Wrote the coverage code for the build_script and  _module_collection_mode_sanitizer functions: Future
Wrote the coverage code for the make_path_spec_relative and 
_check_guts_eq functions: Seleem

