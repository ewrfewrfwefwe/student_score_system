# 学生选课成绩系统
## 课程表 course
| 字段名 | 数据类型 | 约束 | 说明 |
|-------|---------|------|------|
| course_id | int | 主键、非空 | 课程号 |
| course_name | varchar(50) | 非空 | 课程名称 |
| credit | int | 非空 | 学分 |
| tea_id | int | 外键 | 授课教师编号 |

## 选课成绩表 score
| 字段名 | 数据类型 | 约束 | 说明 |
|-------|---------|------|------|
| id | int | 主键、自增 | 记录ID |
| student_id | int | 外键、非空 | 学号 |
| course_id | int | 外键、非空 | 课程号 |
| score | decimal(5,2) |  | 成绩 |