Cling-Locale-Patch
==================

Patch fixing a problem with Cling use of toUpperCase() and toLowerCase() without specifying the correct Locale

Pre-requisite
=============
The Cling library 2.0 snapshot archive

A working Maven installation

Usage
=====

unzip cling-distribution-2.0-SNAPSHOT.zip

cd cling-distribution-2.0-SNAPSHOT

patch -p1 -i <path to cling-locale-patch.diff>

cd core

mvn compile

mvn package

The patched library can be found in core/target
