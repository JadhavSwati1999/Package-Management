# Package-Management
In linux software is available in the form of packages & installing packages means simply extracting files from archive and save it on our system.

Package management is a method to install, upgrade, configure, remove & maintain the software.

Types of Package Manager
Low-level package manager
High-level package manger
In redhat family — rpm (redhat package manager) is used as low-level package manager and yum (yellowdog updater modifier) is used as high-level package manager .
In debian family — — dpm (debian package manager) is used as low-level package manager and apt-get is used as high-level package manager .
rpm (redhat package manager)
rpm only installs the package and not the dependencies.

options -

u = used to upgrade the package
q = query a package
e = erase a package
i = install a package
v = verbose or view
h = hashing
qa = list of all installed pacakge
qd = to view documentation file

Syntax : To install the package

rpm -ivh packagename


syntax : To remove the package

rpm -evh packagename


yum(yellowdog updater modifier)
yum is a open soucre CLI & GUI tool for rpm base system it allows user to install, update or remove or search package on our system.

yum is also used for resolving our dependency issue .

yum does not require complete path to install the package

option

install = to install a package
update =to update a package
list ,listall =specific list or all
info = information of a package
remove =it deletes the packge
auto_remove = it also deletes the dependencies files with the pacakge


Syntax:

yum option packagename -y or -n



Q . Difference between yum and rpm
rpm

RPM stands for RPM Package manager
It doesn’t resolve dependencies, you must install them manually.
This allows you to install multiple versions of the package at once.
When installing a package using the RPM command you must provide the exact location of the “.rpm” package.
RPM is not dependent on YUM
It is difficult to manage RPM in terms of package installation.
RPM doesn’t allow you to upgrade the entire system to the latest available version.
RPM doesn’t allow you to automatically update/upgrade packages installed on your system.
It doesn’t use the online repository to perform any actions.
RPM is a package format and it is a low-level package manager that does basic things.
yum

YUM stands for Yellowdog Updater Modified.

It automatically resolves dependencies and install them simultaneously

This does not allow and shows that the package is already installed.

You can install any package available in the repository, but you only need to know the package name.

It is a frontend tool that uses the RPM package manager on the backend to manage packages.

YUM is the easiest way to manage RPM packages.

YUM allows you to upgrade your system to the latest available version

YUM allows you to automatically update/upgrade the updates available on your system.

It relies entirely on the online repository to do all the work.

This is a top-level front-end package management tool that can do everything you need.

Q . Difference between update and upgrade
update

it makes changes in the existing file or else the existing file is also present and new update file is also stored
upgrade

it directly deletes the existing file and creates the new one according the software
