# mysql_row_number

##### mysql实现一个数据表分数排名的功能



> 创建数据表

```mysql
CREATE TABLE `a` (
`ID` int(10) DEFAULT NULL,
`class` int(10) DEFAULT NULL,
`score` int(10) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8;
```

表格a中字段非常简单，id值，班级id，学生分数

> 插入测试数据

```mysql
INSERT INTO `a` (`ID`, `class`, `score`)
VALUES
(1, 1, 80),
(2, 1, 88),
(3, 1, 90),
(4, 1, 1),
(5, 2, 80),
(6, 2, 22),
(7, 2, 80),
(8, 2, 33),
(9, 2, 65),
(10, 2, 100);
```



> 目前要实现一个功能，对分数进行排名