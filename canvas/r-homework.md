This assessment counts for 50% of your final course mark.

## Note - working together

Please do *not* share answers with anyone else, and do not work with anyone
else on this homework.

Note that we do not use TurnitIn on this homework, but we do other plagiarism
checks.

## Completing the exercise

Like our Zoom session exercises, this exercise uses the R notebook.

You have as long as you want until the due date to work on this homework; you
can search the web and the R documentation for help.

You have the option do to the exercise on your own computer, or on the [R in
the cloud](../pages/R in the cloud) system.

## On your own computer

First, [install R on your computer](../pages/installing-r-on-your-computer).

Next go to [this
link](https://github.com/uob-cfd/rodents/archive/master.zip) to
download a Zip file with the exercise files.

*Unpack the Zip file* to some sensible place on your computer, such as your
Desktop.  See [extracting exercises](../pages/extracting-exercises) for more
detail. In particular, *please don't forget to unpack the zip file*.  This is
especially easy to forget on Windows.  On Windows, make sure, when you open the
Zip file, that you run "Extract All" on the Zip file to extract its contents,
and you then use the extracted files.

Open RStudio, and then use the File - Open File ... option to open the `rodent_survey.Rmd` file.  This is an R notebook.

Fill in the notebook, following the instructions.

Use File - Save to save the notebook when you have finished.

Submit the saved `rodent_survey.Rmd` file here on Canvas.

## On the R in the cloud system

Click on the link below to go to the exercise in the [R in the
cloud](../pages/R in the cloud) system.

[Homework exercise
link](https://uobhub.org/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Fuob-cfd%2Frodents&urlpath=/rstudio)

You will be working on the file `rodent_survey.Rmd` in the `rodents` directory.
See [Work on exercise in R cloud](../pages/work-on-exercise-in-r-cloud) for the
steps to open this file.

Read the instructions in the `rodent_survey.Rmd` notebook and follow them, to
fill in the notebook.

When you have finished, don't forget to [save your
notebook.](../pages/work-on-exercise-in-r-cloud).

Then, [download your saved notebook \".Rmd\" file from the
R cloud](../pages/download-from-r-cloud), and submit the notebook here.

## Problems with the exercise when working on your own computer

Some of you are getting the following error message, when you run the chunk with the code `surveys <- read.csv('rodent_survey_18p2.csv')`:

```
cannot open file 'rodent_survey_18p2.csv': No such file or directoryError in file(file, "rt") : cannot open the connection
```

This happens when, for whatever reason, the file `rodent_survey_18p2.csv` is
not in the same folder as the notebook `.Rmd` file.  There are two common ways this happens:

### You did not extract the files from the Zip archive on Windows

The homework is in a Zip archive (`.zip` file).  By default, if you open this file on Windows, Windows Explorer will show you the Zip file interface.  This shows you the files in the Zip archive, and allows you to open the files *within the Zip archive*, but it does not *extract the files*.   You need to *extract* the files from the Zip archive in their own directory, using the Extract option in the interface.   Then you should open the *extracted* version of the notebook.  If you do not do this, and you are working on the notebook file inside the Zip archive, then you will not have the data file `rodent_survey_18p2.csv` in the same folder, and you will get the error above.  To fix, close the notebook file you are using, make sure you have extracted the Zip archive, and make sure you are using the extracted version of the notebook `.Rmd` file.

### You tried downloading your notebook again from Canvas

Another common reason for this error, is the situation where you filled in the notebook, and everything was working, then you saved the notebook, and submitted via Canvas.  Just to check your submitted file is OK, you download it again from Canvas, but then you run it and get the error above.

The error is because your newly downloaded copy is in a different folder from
your original copy. For example, your new copy might be in your `Downloads`
folder. This folder probably does not contain the `rodent_survey_18p2.csv`
file.   You don't need to fix this - as long as the file that you submitted
works, when you run in its original location, you will be fine, because, when
we mark these files, we make sure the data file is available in the same
folder.  But, if you want to be super-sure, then copy the
`rodent_survey_18p2.csv` file from its original location to the folder
containing your newly downloaded copy of the notebook (such as `Downloads`),
and try running the notebook again.

## Any other problems, on your computer, or on the cloud

Any problems, use the Discussion section on Canvas here, or email
<m.brett@bham.ac.uk>.
