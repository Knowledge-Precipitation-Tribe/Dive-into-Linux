# inode

## inode节点

* Linux操作系统中有一个非常重要的概念叫做inode，中文名为索引节点，目的是为了在物理内存上找到文件块，所以inode中包含文件的相关基本信息澱比如文件位置、文件创建者、创建日期、文件大小等待，输入stat指令可以查看某个文件的inode信息。
* 硬盘格式化的时候，操作系统自动将硬盘分成两个区域，一个是数据区，一个是inode区，存放inode所包含的信息，查看每个硬盘分区的inode总数和已经使用的数量，可以用df命令。
* 在linux系统中，系统内部并不是采用文件名查找文件，而是使用inode编号来识别文件。查找文件分为三个过程：
  * 系统找到这个文件名对应的inode号码
  * 通过inode号码获得inode信息
  * 根据inode信息找到文件数据所在的block读取数据
* 除了文件名之外的所有文件信息都存储在inode中

