##### Code to run at startup of session. Will check for missing packages, install and load them 
library("utils")
Sys.setenv(PATH="/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin")

# Sets the default mirror for downloading and installing packages
print(paste("Setting the default CRAN mirror:","https://cran.rstudio.com/"))
local({
  r <- getOption("repos")
  r["CRAN"] <- "https://cran.rstudio.com/"
  options(repos = r)
})

# Checks, installs and loads packages from list below
cPackageList = c("shiny","shinydashboard","snowfall","rlecuyer",
	"data.table","ggplot2","scales","RSQLite","googlesheets","signal","dplyr","plyr","zoo")

fCheckInstallPackages <- function(packageName){
	if(!require(packageName,character.only=TRUE)){
		install.packages(packageName)
	}
	library(packageName,character.only=TRUE)
}

sapply(cPackageList,fCheckInstallPackages)
