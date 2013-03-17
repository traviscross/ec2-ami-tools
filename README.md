# Debian Packaging for Amazon AMI Tools

This repository contains debian packaging for the
[Amazon EC2 AMI Tools](http://aws.amazon.com/developertools/368), which
are command-line utilities that help create and manage Amazon Machine
Images (AMIs).

If you wish to use `dpkg`, `apt`, or `aptitude` to install the Amazon
AMI Tools on a [Debian](http://www.debian.org/) system, then you might
be interested in this packaging.

## Usage

### Building the Debian binary packages only

To build the debs, checkout the `debian` branch and run:

    dpkg-buildpackage -b -us -uc

### Building the Debian source package

To build the source package and debs, checkout the `debian` branch and
run:

    ./debian/mkorig.sh origin/upstream
    dpkg-buildpackage -us -uc

## See also

Please also read the contents of the files `debian/README.source` and
`debian/README.Debian`.
