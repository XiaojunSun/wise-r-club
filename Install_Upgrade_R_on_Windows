# Install and Upgrade R on Windows

WISE R CLUB, Xiaojun Sun, 2014.06.20

R is a language and environment for statistical computing and graphics. It is widely used around the world. Here I briefly describe the steps to install and upgrade R for R beginners. 

## Step 1: Download R and Rstudio
The latest version of R can be download from [CRAN][2]. Rstudio Desktop can be download from it's [official site][3]. 

![Rstudio](http://i.imgbox.com/IHpsi4Gn.png "Download Rstudio")

Now install R first.

![installR01](http://i.imgbox.com/IRTRIvg5.jpg "Choose directory to install R")

![installR02](http://i.imgbox.com/fo9YGrzg.jpg "Choose according to you PC system")

If you install it successfully, you open R and will see this:
![installR03](http://i.imgbox.com/5aw3DW4B.jpg "R windows") 

Then install Rstudio Desktop.

![installRstudion1](http://i.imgbox.com/exN40Tst.jpg "Choose directory to install Rstudio")

Open Rstudio you will see this.
![installRstudion2](http://i.imgbox.com/W5BWO12s.jpg "Rstudio Interface")


## Step 2: Upgrade R
Now we set up the global library for R. More details about this is described in [Tal Galili's blog post][1].

Open your R. Run `chooseMirror()` command line(Type it and hit `ENTER`) .Choose `China(Xiamen)`.

![mirror](http://i.imgbox.com/nMC12nzx.jpg "Choose Mirror")

Run the following codes line by line.
```
source("http://www.r-statistics.com/wp-content/uploads/2010/04/upgrading-R-on-windows.r.txt")
# Hit `ENTER` to run the command.
Old.R.RunMe()
```
![oldr](http://i.imgbox.com/yn5SmnIH.jpg "Set global lib")

It will ask you whether or not to quit R. Just type `n` and hit `ENTER`. Then run `New.R.RunMe()` just the same way.


Once you have done these, from now on, whenever you want to update to a new version of R in the future, all you will need to do are the following **TWO** steps:

1. Download and install the new version of R
2. Open your new R and run the following codes

```
source("http://www.r-statistics.com/wp-content/uploads/2010/04/upgrading-R-on-windows.r.txt")
New.R.RunMe()
```

That's all. I hope it helps. Thank you! O(∩_∩)O


[1]: http://www.r-statistics.com/2010/04/changing-your-r-upgrading-strategy-and-the-r-code-to-do-it-on-windows/
[2]: http://mirrors.xmu.edu.cn/CRAN/
[3]: http://www.rstudio.com/products/rstudio/download/
