# Boston_Crimes
Data at
dir.create( "dropbox" )
download.file(" https://www.dropbox.com/s/jqlcl79p5q1yvb2/crime.csv?dl=1", 
              "./dropbox/crime.csv" )
             
dat2 <- read.csv( "./dropbox/crime.csv" )


# deletes downloaded file
file.remove( "./dropbox/crime.csv" )


# deletes entire directory
unlink( "dropbox", recursive = TRUE )
