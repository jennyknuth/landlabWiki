  <p>
    This should work for <a href="https://www.continuum.io/downloads">Anaconda</a> users with Windows 7+, Mac OS 10.6+, or Ubuntu
    Linux (only the latest version has been tested).
  </p>

  <p>
    Once you have <a href="http://landlab.readthedocs.org/en/latest/install.html#installing-python">a full Python distribution on your machine</a>, it is vital to
    check that it has been successfully set as the default copy of Python on
    your system. Open a command prompt (Terminal on a Mac, or Command Prompt
    on a PC) and type the lines below (note the <code>></code> indicates that you are on a
    command line):
  </p>

  <p>
   <code>
     > which python
   </code>
  </p>
  <p>
   <code>
     > which ipython
   </code>
  </p>
  <p>
    In each case, the path should be the same, and it should clearly refer to Anaconda (or
    Canopy). Details will depend on your operating system but it could look something like this:
  </p>

  <p>
   <code>
     /anaconda/bin/python
   </code>
  </p>
  <p>
    If you don’t see reference to your newly installed
    distribution (i.e., <code>/anaconda</code>), <a href="http://landlab.readthedocs.org/en/latest/correcting_python_version.html#correcting-python-version">click here</a> to resolve the problem.
  </p>

  <p>
    Once the path to both <code>python</code> and
    <code>ipython</code> point to your new distribution, open the
    Python editor in Anaconda called Spyder.
  </p>

  <p>
    On the Spyder toolbar, go to <code>Tools → Open</code> command prompt to open the command
    line.
  <p>

  </p>
    Alternatively you can open a standard terminal window, such as an
    xterm (X11.app) or terminal window (Terminal.app) on a Mac, or a command
    prompt on a Windows machine. If you do use a standard terminal and run into
    problems, make sure you have <a href="http://landlab.readthedocs.org/en/latest/correcting_python_version.html#correcting-python-version">resolved your path issues.</a>
  </p>

  <p>
    Ensure that your version of pip (a package installer) is up-to-date by typing:
  </p>

  <p>
    <code>
      > pip install --upgrade pip
    </code>
  </p>

  <p>
    Next, make sure the necessary dependencies are
    up-to-date. The following <code>conda</code> command will update (almost) all Anaconda packages
    (Note the conda command below handles Anaconda-supported package
    installation and updates):
  </p>

  <p>
    <code>
      > conda update --all
    </code>
  </p>
  <p>
    Installing also requires a fully up-to-date version of
    <code>setuptools,</code> which (irritatingly) is not updated by the <code>update --all</code> command above. So
    also run:
  </p>

  <p>
    <code>
      > conda update setuptools
    </code>
  </p>

  <p>
    Once the Anaconda packages are updated and the
    correct version of pip is installed, now install <code>netCDF4</code>:
  </p>

  <p>
    <code>
      > conda install netCDF4
    </code>
  </p>

  <p>
    Now to install Landlab! Enter the following command:
  </p>

  <p>
    <code>
      > pip install landlab
    </code>
  </p>

  <p>
    Once Landlab has been successfully installed, on the
    Python shell line, check to make sure it is up-to-date (note that those are
    double underscores around version; also note that you may need to close and
    reopen Anaconda before typing the below commands):
  </p>

  <p>
    <code>
      > import landlab
    </code>
  </p>
  <p>
    <code>
      > landlab.__version__
    </code>
  </p>

   <p>
     The version number is changing rapidly at this point, but it should be
     something higher than 0.1.18.
   </p>

   <p>
     If you are having problems with Landlab, check with the Landlab
     development team to make sure you have the latest version.
   </p>
