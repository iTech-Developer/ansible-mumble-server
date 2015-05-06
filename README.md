mumble-server
=============

Ansible role that installs and configures Murmur on a debian server.

Role Variables
--------------

There are 52 role variables available, one for every single Murmur configuration option that can be set. All variables and default values can be found in the `default/mumble-server.ini.j2` template. 

List of variables and description can be found on [mumble wiki](http://wiki.mumble.info/wiki/Murmur.ini)

The role will set a default SuperUser password, you will need to override **murmur_superuser** with your password. Also *murmur_icesecretread* and *murmur_icesecretwrite* have a randomly generated default password.

If UFW is installed, a rule will be added to allow the murmur port

License
-------

The MIT License (MIT)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
