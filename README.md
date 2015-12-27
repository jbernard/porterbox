A simple script to list the available debian porterbox machines.  If you happen
to be a debian developer and you need access to a particular architecture, this
script might be helpful if you don't feel like reading the web page. 

The output looks similar to:

    Architecture       Hostname                 Access
    --------------------------------------------------------------------
    armel              abel.debian.org          public
    armhf              asachi.debian.org        public
    kfreebsd-amd64     asdfasdf.debian.net      public (non-DSA-machine)
    amd64              barriere.debian.org      restricted
    mipsel             eder.debian.org          public
    hurd-i386          exodar.debian.net        public (non-DSA-machine)
    kfreebsd-amd64     falla.debian.org         public
    kfreebsd-i386      fischer.debian.org       public
    mips               gabrielli.debian.org     public
    armhf              harris.debian.org        [unknown]
    kfreebsd-i386      io.debian.net            public (non-DSA-machine)
    armhf              ipa.debian.net           public (non-DSA-machine)
    ia64               merulo.debian.org        public
    powerpc            partch.debian.org        developer only
    ppc64el            pastel.debian.net        public (non-DSA-machine)
    sh4                sh4.g15.jp               public (non-DSA-machine)
    sparc              smetana.debian.org       public
    hurd-i386          strauss.debian.net       public (non-DSA-machine)
    sh4                sumotsu.debian.net       public (non-DSA-machine)
    armhf              turfan.debian.net        public (non-DSA-machine)
    avr32              xoothais.err.no          public (non-DSA-machine)
    s390x              zelenka.debian.org       public

    Found 22 machines

## Installation

You can use pip directly from the cloned repository:

    $ cd porterbox
    $ pip install -r requirements.txt
    $ pip install . (or run the script directly)

Or you can create a virtualenv and install there (make sure `python-virtualenv`
is installed):

    $ cd porterbox
    $ virtualenv .venv
    $ . .venv/bin/activate
    $ pip install -r requirements.txt
    $ pip install . (or run the script directly)
