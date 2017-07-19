This is a model project which I use.
The folder arrangement is indebted to ???
I have also downloaded the github bookdown repo, removed the .Rproj file, and moved the Rmd file to the sandbox folder in the first instance. 

The central ideas are that the Rmd file go first to sandbox, and eventually to reports. The Rchunks folder holds one file, and the function_library holds only one file. 
In function_library you find only function definitions. In Rchunks you find ony invocation of extant R functions, or calls to functions defined in the function library.  The Rchunks file uses the "R chunks" format with a 
# ---- NAME ------
style delimiting various activities.

The first few chunks in the Rchunks.R are my default set-up functions. Note carefully how figures and tables are constructed, captions, etc. I have found this particularly sensitive to purtubation.

You write the text in the sandbox folder, dividing the chapters up as you see fit. Note how the first function call in the index.Rmd file sources the helper_function library and reads the Rchunks file.  This is an explicit reference so if you change the name of the helper_function file, or the Rchunks library, you have to change it is the sandbox/index.Rmd file.

I have found bookdown very helpful