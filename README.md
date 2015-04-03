# xar
Attempt to use click
Lists all servers/lb/block storage/database resources in Rackspace Cloud.

Only partially works since I stopped working on it. 

python allxar list - works

click (4.0)
pyrax (1.9.2)

Example:

# python allxar list
+---------+-------------------------+--------------------------------------+--------+-----------------+----------------+--------+
| Service | Name                    | ID                                   | Status | Public IP       | Private IP     | Region |
+---------+-------------------------+--------------------------------------+--------+-----------------+----------------+--------+
| Servers | testing-tools-dfw       | 6a9b0d5c-34d4-4ae4-bed3-f6e08b0afedd | ACTIVE | 100.100.100.100 | 10.208.100.100 | DFW    |
| Servers | Cloud-Server-01         | baf0242b-9e11-40e7-ab51-484a89868cf4 | ACTIVE | 100.100.100.100 | 10.208.100.100 | DFW    |
| Servers | Cloud-Server-18         | ae664bc2-8703-4798-a29e-686fac13f8ea | ACTIVE | 100.100.100.100 | 10.208.100.100 | DFW    |
| Servers | iad                     | 5d36f87c-f864-48ce-812c-7d7dbe54feb1 | ACTIVE | 100.100.100.100 | 10.208.100.100 | IAD    |
| Servers | Cloud-Server-06         | e50ae40a-0bbc-4cc2-bde6-2e933611f89c | ACTIVE | 100.100.100.100 | 10.208.100.100 | ORD    |
| Servers | Cloud-Server-10         | b2059092-1e1b-4c5d-9801-cd841e73c481 | ACTIVE | 100.100.100.100 | 10.208.100.100 | ORD    |
| Servers | CruOS 6                 | a404fc56-97b1-4378-b8fa-7e76bd9945fb | ACTIVE | 100.100.100.100 | 10.208.100.100 | ORD    |
| Servers | Cloud-Server-12         | 284b9b1f-6056-4312-a239-cba6574b4da5 | ACTIVE | 100.100.100.100 | 10.208.100.100 | ORD    |
| Servers | Cloud-Server-11         | 6fa5166b-2490-4081-b5c6-6252eb9bac2f | ACTIVE | 100.100.100.100 | 10.208.100.100 | ORD    |
| Servers | Cloud-Server-09         | aed686cc-f491-4677-9b6a-a2438feca0fe | ACTIVE | 100.100.100.100 | 10.208.100.100 | SYD    |
| Servers | Cloud-Server-15         | 211e75c8-5d25-4964-947f-b845e5236017 | ACTIVE | 100.100.100.100 | 10.208.100.100 | SYD    |
+---------+-------------------------+--------------------------------------+--------+-----------------+----------------+--------+
+-----------+-------------+--------------------------------------+--------+--------+
|  Service  |     Name    |                  ID                  | Status | Region |
+-----------+-------------+--------------------------------------+--------+--------+
| Databases | Instance-02 | 43d8327b-fe4a-491e-aba3-447729056088 | ACTIVE |  DFW   |
+-----------+-------------+--------------------------------------+--------+--------+
+----------------+--------------+--------+--------+--------+
| Service        | Name         | ID     | Status | Region |
+----------------+--------------+--------+--------+--------+
| Load Balancers | autoscale-LB | 237935 | ACTIVE | DFW    |
+----------------+--------------+--------+--------+--------+
+---------------+---------------+--------------------------------------+-----------+--------+
| Service       | Name          | ID                                   | Status    | Region |
+---------------+---------------+--------------------------------------+-----------+--------+
| Block Storage | lvm           | 1ec87988-0895-4cc1-8e10-029d9f7ae2eb | in-use    | DFW    |
| Block Storage | ripdisk       | 42fb07f0-5a8d-48c4-b041-c3628203b7a7 | available | DFW    |
| Block Storage | Storage       | 48997667-36eb-4212-931d-ca8f46c6294b | in-use    | DFW    |
| Block Storage | sh.test       | d60a3293-3e40-4cd5-82cd-421a3d3ff202 | available | IAD    |
| Block Storage | test          | f16e767d-ee75-4ec1-a87f-9887d2b02386 | in-use    | ORD    |
+---------------+---------------+--------------------------------------+-----------+--------+
