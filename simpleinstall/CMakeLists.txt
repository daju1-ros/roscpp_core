cmake_minimum_required(VERSION 2.8)

install(PROGRAMS simpleinstall_bin.py
  DESTINATION bin)

add_subdirectory(src)


# need your gpg keys set up and gpg-agent on
# debuild -S to build source package
# dput ppa:straszheim/ros ../simpleinstall_x.y.y_source.changes
# dpkg-buildpackage will make a deb
# DEBFULLNAME="Troy Straszheim" DEBEMAIL="straszheim@willowgarage.com" dch -l bazinga   (bazinga is suffix to be added to version number.  
#                   trailing digits added automagically)

# distros in changelog:  multiples don't be working.

