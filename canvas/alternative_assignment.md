This exercise uses the R notebook.

See the [Zoom session on the
R notebook](../pages/zoom-session-introduction-to-r-notebook) page for more
details about how to use the R notebook.

You might also want to have a look at [this video on using the R
notebook](https://vimeo.com/319738376).

You should do the exercise on your own computer.

Make sure you have [installed R on your
computer](../pages/installing-r-on-your-computer).

Next go to [this
link](https://github.com/uob-cfd/more_gender_data/archive/main.zip)
to download a Zip file with the exercise files.

*Unpack the Zip file* to some sensible place on your computer, such as
your Desktop. *Please don't forget to unpack the zip file*. This is
especially easy to forget on Windows. On Windows, make sure, when you
open the Zip file, that you run "Extract All" on the Zip file to extract
its contents, and you then use the extracted files.

Open RStudio, and then use the File - Open File ... option to open the
`more_gender_data.Rmd` file. This is an R notebook.

Fill in the notebook, following the instructions.

Use File - Save to save the notebook when you have finished.

Submit the saved `more_gender_data.Rmd` file here on Canvas.

Don't worry about the filename - any filename will work. Canvas makes a
unique filename for us when we download the files for marking.

**Please see section below on errors you may see if you re-download your
notebook from Canvas**.

## Troubleshooting {#problems-with-the-exercise-when-working-on-your-own-computer}

Some of you are getting the following error message, when you run the
chunk with the code `gender_data <- read.csv('gender_stats.csv')`:

    cannot open file 'gender_stats.csv': No such file or directoryError in file(file, "rt") : cannot open the connection

This happens when, for whatever reason, the file `gender_stats.csv`
is not in the same folder as the notebook `.Rmd` file.

There are two common ways this happens --- see the sections below.

See the section below that for instructions on fixing the error.

### You did not extract the files from the Zip archive on Windows

The homework is in a Zip archive (`.zip` file). By default, if you open
this file on Windows, Windows Explorer will show you the Zip file
interface. This shows you the files in the Zip archive, and allows you
to open the files *within the Zip archive*, but it does not *extract the
files*. You need to *extract* the files from the Zip archive in their
own directory, using the Extract option in the interface. Then you
should open the *extracted* version of the notebook. If you do not do
this, and you are working on the notebook file inside the Zip archive,
then you will not have the data file `gender_stats.csv` in the same
folder, and you will get the error above. To fix, close the notebook
file you are using, make sure you have extracted the Zip archive, and
make sure you are using the extracted version of the notebook `.Rmd`
file.

### You tried downloading your notebook again from Canvas

Another common reason for this error, is the situation where you filled
in the notebook, and everything was working, then you saved the
notebook, and submitted via Canvas. Just to check your submitted file is
OK, you download it again from Canvas, but then you run it and get the
error above.

The error is because your newly downloaded copy is in a different folder
from your original copy. For example, your new copy might be in your
`Downloads` folder. This folder probably does not contain the
`gender_stats.csv` file. You don't need to fix this - as long as
the file that you submitted works, when you run in its original
location, you will be fine, because, when we mark these files, we make
sure the data file is available in the same folder. But, if you want to
be super-sure, then copy the `gender_stats.csv` file from its
original location to the folder containing your newly downloaded copy of
the notebook (such as `Downloads`), and try running the notebook again.

### Fixing "cannot open the connection" errors

Please read the text above this for why you are getting this error.

See the [connection fix
video](https://bham.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=8d78aa93-2ad3-4cd4-86b7-ad1f00a49537)
for instructions on diagnosing and fixing the error.

## Any other problems {#any-other-problems-on-your-computer-or-on-the-cloud}

Any problems, use the Discussion section on Canvas here, or email
<m.brett@bham.ac.uk>.
