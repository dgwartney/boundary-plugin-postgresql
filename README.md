Boundary PostgreSQL Plugin
--------------------------
**Awaiting Certification**

Extracts metrics from a PostgreSQL database instance.



Prerequisites
-------------
The following items are required on the host platform in addition to the Boundary Premium [relay](http://premium-support.boundary.com/customer/portal/articles/1635550-plugins---how-to).
- Python 2.6.6 or later
- PsycoPG2 module
- PostreSQL development packages: postgresql-devel
- Python development packages: python-devel

### Plugin Setup

#### Installation of the PsycoPG2 Library Using `pip`

1. Install [pip](http://pip.readthedocs.org/en/latest/installing.html) if not already installed

     ```bash
      $ curl -s https://bootstrap.pypa.io/get-pip.py > get-pip.py
      $ sudo python get-pip.py
     ```
2. Install the `psycopy2` module

     ```bash
      $ pip install psycopg2
     ```

### Plugin Configuration Fields
|Field Name|Description                                       |
|:-------|:-------------------------------------------------|
|host    |database host name or IP                          |
|port    |PostgreSQL Port                                   |
|database|database name                                     |
|username|PostgreSQL username                               |
|password|PostgreSQL Password (if not required put anything)|
|source  |display name                                      |

### Metrics Collected

|Metric Name                                    |Description                                    |
|:----------------------------------------------|:----------------------------------------------|
|PostgreSQL - Locks Exclusive                   |PostgreSQL - Locks Exclusive                   |
|PostgreSQL - Locks Row Exclusive               |PostgreSQL - Locks Row Exclusive               |
|PostgreSQL - Locks Share Row Exclusive         |PostgreSQL - Locks Share Row Exclusive         |
|PostgreSQL - Locks Share Update Exclusive Locks|PostgreSQL - Locks Share Update Exclusive Locks|
|PostgreSQL - Locks Share                       |PostgreSQL - Locks Share                       |
|PostgreSQL - Locks Access Share                |PostgreSQL - Locks Access Share                |
|PostgreSQL - Checkpoint Write Time             |PostgreSQL Checkpoint Write Time               |
|PostgreSQL - Checkpoints Timed                 |PostgreSQL - Checkpoints Timed                 |
|PostgreSQL - Buffers Allocated                 |PostgreSQL Buffers Allocated                   |
|PostgreSQL - Buffers Clean                     |PostgreSQL - Buffers Clean                     |
|PostgreSQL - Buffers Backend Fsync             |PostgreSQL - Buffers Backend Fsync             |
|PostgreSQL - Checkpoint Synchronization Time   |PostgreSQL - Checkpoint Synchronization Time   |
|PostgreSQL - Checkpoints Requested             |PostgreSQL - Checkpoints Requested             |
|PostgreSQL - Buffers Backend                   |PostgreSQL - Buffers Backend                   |
|PostgreSQL - Maximum Written Clean             |PostgreSQL - Maximum Written Clean             |
|PostgreSQL - Buffers Checkpoint                |PostgreSQL - Buffers Checkpoint                |
|PostgreSQL - Blocks Read                       |PostgreSQL - Blocks Read                       |
|PostgreSQL - Disk Size                         |PostgreSQL - Disk Size                         |
|PostgreSQL - Transaction Committed             |PostgreSQL - Transaction Committed             |
|PostgreSQL - Transactions Rolledback           |PostgreSQL - Transactions Rolledback           |
|PostgreSQL - Blocks Hit                        |PostgreSQL - Blocks Hit                        |
|PostgreSQL - Tuples Deleted                    |PostgreSQL - Tuples Deleted                    |
|PostgreSQL - Tuples Fetched                    |PostgreSQL - Tuples Fetched                    |
|PostgreSQL - Tuples Inserted                   |PostgreSQL - Tuples Inserted                   |
|PostgreSQL - Tuples Returned                   |PostgreSQL - Tuples Returned                   |
|PostgreSQL - Tuples Updated                    |PostgreSQL - Tuples Updated                    |

