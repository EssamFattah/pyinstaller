<img width="962" alt="Screenshot 2024-06-27 at 8 18 29 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/714a35ae-b9c4-46fd-a54c-bedcddfc2a59"># Report for Assignment 1

## Project chosen

Name: Pyinstaller

URL: https://github.com/EssamFattah/pyinstaller.git

Number of lines of code and the tool used to count it: 60,825 TOTAL, 42,000 written in Python (used lizard to count)

Programming language: Python

## Coverage measurement

### Existing tool

After downloading the necessary modules from the requirements.txt file using “pip install -r requirements.txt”, we used the Coverage.py command  “coverage run --source=. -m pytest” to test the coverage of our code. We then translated the results into HTML to help us better visualise the coverage using “coverage html”:

<img width="791" alt="1" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/91b60355-69a6-43b6-b7d3-ee1e60f4bda5">

<img width="797" alt="Screenshot 2024-06-27 at 8 17 29 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/cc0fc79f-033e-446f-b350-042a76ff762c">

We find a coverage of 60 percent for the project.

### Your own coverage tool

Future (Essam) Abdel Fattah:

Function 1 name: build_script(text_options=None, always_on_top=False)

<img width="967" alt="Screenshot 2024-06-27 at 8 19 08 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/ec315f5c-87c9-4a59-ba3a-bd8b846e65bb">


Commit link: https://github.com/pyinstaller/pyinstaller/commit/b0aacbd4fd1e696b1157b3e74dad9238b00b7b10#



Function 2 name:  _module_collection_mode_sanitizer(value)

<img width="944" alt="Screenshot 2024-06-27 at 8 19 23 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/9fdda14f-408f-4d65-a2dd-04df78d6723e">

Commit link:
https://github.com/pyinstaller/pyinstaller/commit/9e222041cd34a99393c73905675d422f3ea1b8dc

Member 2 Seleem Wagdy:

Function 1 name: make_path_spec_relative(filename, spec_dir)

<img width="942" alt="Screenshot 2024-06-27 at 8 19 40 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/94e60348-e11d-4820-ba1f-1ccb8273561c">

Commit link:
https://github.com/pyinstaller/pyinstaller/commit/664f977348b4e57cd3422dc6b985e3b82cdd4657

Function 2 name:  _check_guts_eq(attr_name, old_value, new_value, last_build)

 <img width="939" alt="Screenshot 2024-06-27 at 8 19 53 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/f739a871-1635-4d68-be6b-fa728cba447b">

Commit link:
https://github.com/pyinstaller/pyinstaller/commit/fb1013de80eadff211f11ac69d2f5e3aa280b621

## Coverage improvement

### Individual tests

Member 1 Future (Essam) Abdel Fattah:
Test 1:

Commit: https://github.com/pyinstaller/pyinstaller/commit/b0aacbd4fd1e696b1157b3e74dad9238b00b7b10#

Old coverage results:

<img width="724" alt="Screenshot 2024-06-27 at 8 20 21 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/1001c6ee-f912-4b43-8b73-343234ccdf04">


New coverage results:

<img width="917" alt="Screenshot 2024-06-27 at 8 20 38 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/798bf246-8b71-44e3-a5e7-0938bc4f2a70">


We created a test case where the font is “TKDefault” as well as a test case where the font is “Helvetica”, this made sure that the code in the conditional statements is covered. We can see this is the case because of the green highlight seen in the screenshot above.

<img width="753" alt="Screenshot 2024-06-27 at 8 20 56 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/ab1093ac-44b5-4561-9cbc-b86f3aca6dc9">



Test 2:

Old coverage results:

<img width="934" alt="Screenshot 2024-06-27 at 8 21 11 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/72970b8a-6234-424b-a351-0853b98524a7">

New coverage results:

<img width="939" alt="Screenshot 2024-06-27 at 8 21 23 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/b3b2f3d2-6305-4bc6-b5b0-75cdb24d4605">


We created 2 test cases to cover both of the branches seen in the code, the first test case tests when value is a dictionary variable, and the second test case tests when value is a string variable. This properly covers both available branches of the function.

<img width="786" alt="Screenshot 2024-06-27 at 8 21 34 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/7e83568f-11e7-4b8a-8c3a-55eab21e734e">

Commit link:
https://github.com/pyinstaller/pyinstaller/commit/9e222041cd34a99393c73905675d422f3ea1b8dc


Member 2: Seleem Wagdy

Test 1:
<Show a patch (diff) or a link to a commit made in your forked repository that shows the new/enhanced test>

  Old coverage:
 
  <img width="847" alt="Screenshot 2024-06-27 at 8 21 49 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/ff3c22f8-ed73-4db5-ad44-ae48ea9e6f2c">

	
  New coverage:
  
	<img width="944" alt="Screenshot 2024-06-27 at 8 22 07 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/6be200df-136b-42af-b23a-a7fa7af2e37e">


For this function, we created two test cases that would cover the available branches. The first case takes filename to be an absolute path (“//”), while the second test case takes to be a normal path (“C:”).

<img width="778" alt="Screenshot 2024-06-27 at 8 22 23 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/31a027e5-6f23-4b19-ac56-37905ccdb5df">


Commit link:
https://github.com/pyinstaller/pyinstaller/commit/664f977348b4e57cd3422dc6b985e3b82cdd4657

Task 2:

Old coverage: 

<img width="944" alt="Screenshot 2024-06-27 at 8 22 36 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/658e7079-6dca-408f-b214-83595a19f85a">

New coverage:

<img width="946" alt="Screenshot 2024-06-27 at 8 22 54 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/9530ee29-756f-4e11-afb6-f101916cd5c2">

We created two test cases to cover both branches present in this function, first we created a test cases where old_value and new_value are different, and a test case where they are the same.

<img width="694" alt="Screenshot 2024-06-27 at 8 23 03 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/204eca72-cd77-459a-bef0-16f4fd057faa">

Commit link:
https://github.com/pyinstaller/pyinstaller/commit/fb1013de80eadff211f11ac69d2f5e3aa280b621

### Overall

Old coverage:

<img width="795" alt="Screenshot 2024-06-27 at 8 23 14 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/169dd72e-56f9-48cc-9d53-8626c0d2bbd7">

New coverage:

<img width="944" alt="Screenshot 2024-06-27 at 8 23 24 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/52bacb4e-3ab7-43a7-9b2f-2492fdaf8c44">

We can see a coverage increase of 1% on the overall code, down below you can see the individual files that were modified, and how their coverage was affected after our tests were implemented.

<img width="915" alt="Screenshot 2024-06-27 at 8 23 44 PM" src="https://github.com/EssamFattah/pyinstaller/assets/122282163/ab592024-db1d-4b19-bc39-dd568b592088">

## Statement of individual contributions
Looked for a suitable repository: Future and Seleem
Figured out how to run the coverage test: Future and Seleem
Took care of the forked repository: Future
Wrote and put together the documentation: Seleem
Wrote the coverage code for the build_script and  _module_collection_mode_sanitizer functions: Future
Wrote the coverage code for the make_path_spec_relative and 
_check_guts_eq functions: Seleem

