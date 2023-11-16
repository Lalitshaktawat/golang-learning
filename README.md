**Go** is also referred to as Golang, it is a free and open-source programming language designed at Google by Robert Griesemer, Rob Pike, and Ken Thompson. It is an apple to many a developer’s eye due to its simplicity, efficiency, and concurrency. Its concurrent nature implies means its ability to run multiple tasks at the same time.

It is mostly used for backend purposes such as server-side programming. It features majorly in the game and cloud-native development,  development of command-line tools, data science, and many more use cases.

## Install Go from the Official Binary Package

This is the most preferred installation method as it provides the latest version of Golang Go and cuts across all Linux distributions. To achieve this, follow the steps outlined.

### Step 1:  Download the Go

The first step in installing Go is to update the system. So log in to your server and update the local package index as shown.

```R
$ sudo apt update
```

### Step 2:  Download the Go Binary Package

The next step is to download the installation file which is a tarball file. To download it, head over to the official Go download page and download the 64-bit tarball installation file ( amd64.tar.gz )

On the command line, you can download the latest tarball file using the wget command. At the time of writing this guide, the latest version of Go is Go 1.20.1. This is likely to change by the time you are reading this guide, so ensure to replace the version number accordingly.

[Go lang version](https://go.dev/dl/)

```R
$ wget https://go.dev/dl/go1.21.4.linux-amd64.tar.gz
```

### Step 3:  Unzip the tarball file & move it to /usr/local directory

Once the download is complete, unzip the tarball to the ==**/usr/local/**== directory which is the primary directory for executable files.

```R
$ sudo tar -C /usr/local -xzf go1.21.4.linux-amd64.tar.gz
```

The -C option uncompresses the contents of the tarball file to the /usr/local directory inside the go folder. To confirm this, list the contents of the **/usr/local/** directory using the ls command.

```R
$ ls /usr/local/go
```

### Step 4: Add the Golang binary to the $PATH environment variable

The next step is to add Go to the $PATH environment variable.

Open up your **.bashrc** or **.bash_profile / .profile** file.

```R
$ vi ~/.bash_profile
```

Paste the following line.

```R
export PATH=$PATH:/usr/local/go/bin
```

Save the changes and exit the file.

Next, reload the  .bashrc or .bash_profile file using the source command as shown.

```R
$ source ~/.bash_profile
```

Now Go is successfully installed.

### Step 5: Verify Go Version

To check if Go is installed and its version, run the command:

```R
$ go version
```
