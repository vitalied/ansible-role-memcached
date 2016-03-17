Ansible Role for Memcached
====================

[![Build Status](https://travis-ci.org/vitalied/ansible-role-memcached.svg?branch=master)](https://travis-ci.org/vitalied/ansible-role-memcached)
[![GitHub tag](https://img.shields.io/github/tag/vitalied/ansible-role-memcached.svg)](https://github.com/vitalied/ansible-role-memcached)
[![GitHub license](https://img.shields.io/github/license/vitalied/ansible-role-memcached.svg)](https://github.com/vitalied/ansible-role-memcached/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/ansible/role/8579.svg)](https://galaxy.ansible.com/vitalied/memcached)

Ansible Role for Memcached Management.

Requirements
------------

This role require Ansible 2.1 or higher.

This role was designed for Ubuntu Server 14.04+.

Role Variables
--------------

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>parameter</th>
<th>required</th>
<th>default</th>
<th>choices</th>
<th>comments</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>memcached_user</td>
<td>yes</td>
<td>memcached</td>
<td></td>
<td>The user under which the Memcached daemon will run.</td>
</tr>
<tr class="even">
<td>memcached_listen_ip</td>
<td>yes</td>
<td>127.0.0.1</td>
<td></td>
<td>The IP address (127.0.0.1 for localhost) on which memcached will listen for requests.</td>
</tr>
<tr class="odd">
<td>memcached_port</td>
<td>yes</td>
<td>11211</td>
<td></td>
<td>The port on which memcached will listen for requests.</td>
</tr>
<tr class="even">
<td>memcached_memory_limit</td>
<td>yes</td>
<td>64</td>
<td></td>
<td>The maximum amount of RAM memcached will consume.</td>
</tr>
<tr class="odd">
<td>memcached_max_connections</td>
<td>yes</td>
<td>1024</td>
<td></td>
<td>The maximum number of simultaneous connections memcached will handle.</td>
</tr>
</tbody>
</table>

Dependencies
------------

No additional role dependencies.

Example Playbook
----------------

    - hosts: all
      roles:
        - role: vitalied.memcached

License
-------

-   Code released under [MIT](https://github.com/vitalied/ansible-role-memcached/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)
