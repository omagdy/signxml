
This is a forked version of the Signxml Repositry (https://github.com/XML-Security/signxml) which is slightly adjusted to fit a project need.

Installation guide:

Note: SignXML depends on `lxml <https://github.com/lxml/lxml>`_ and `cryptography
<https://github.com/pyca/cryptography>`_, which in turn depend on `OpenSSL <https://www.openssl.org/>`_, `LibXML
<http://xmlsoft.org/>`_, and Python tools to interface with them. You can install those as follows:

+--------------+---------+-------------------------------------------------------------------------------------------------+
| OS           | Python  | Command                                                                                         |
+==============+=========+=================================================================================================+
| Ubuntu 16.04 | Python 2| ``apt-get install python-dev python-cffi libxml2-dev libxslt1-dev libssl-dev``                  |
|              |         | ``python-lxml python-cryptography python-openssl python-certifi python-defusedxml``             |
+--------------+---------+-------------------------------------------------------------------------------------------------+
| Ubuntu 16.04 | Python 3| ``apt-get install python3-dev python3-cffi libxml2-dev libxslt1-dev libssl-dev``                |
|              |         | ``python3-lxml python3-cryptography python3-openssl python3-certifi python3-defusedxml``        |
+--------------+---------+-------------------------------------------------------------------------------------------------+
| Ubuntu 14.04 | Python 2| ``apt-get install python-dev python-cffi libxml2-dev libxslt1-dev libssl-dev``                  |
+--------------+---------+-------------------------------------------------------------------------------------------------+
| Ubuntu 14.04 | Python 3| ``apt-get install python3-dev python3-cffi libxml2-dev libxslt1-dev libssl-dev``                |
+--------------+---------+-------------------------------------------------------------------------------------------------+
| Ubuntu 12.04 | Python 2| ``apt-get install python-dev libxml2-dev libxslt1-dev libssl-dev; pip install cffi``            |
+--------------+---------+-------------------------------------------------------------------------------------------------+
| Red Hat      | Python 2| ``yum install python-devel python-cffi libxml2-devel libxslt1-devel openssl-devel``             |
+--------------+---------+-------------------------------------------------------------------------------------------------+
| Red Hat      | Python 3| ``yum install python3-devel python3-cffi libxml2-devel libxslt1-devel openssl-devel``           |
+--------------+---------+-------------------------------------------------------------------------------------------------+
| OS X/Homebrew|         | ``xcode-select --install; brew install openssl;``                                               |
|              |         | ``export LDFLAGS="-L$(brew --prefix openssl)/lib" CFLAGS="-I$(brew --prefix openssl)/include"`` |
+--------------+---------+-------------------------------------------------------------------------------------------------+

sudo pip install -e git+https://github.com/omagdy/signxml#egg=signxml
