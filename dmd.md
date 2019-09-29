# ��һ����ѯ���
* SELECT d.department_name,count(e.job_id)as "����������",
avg(e.salary)as "ƽ������"
from hr.departments d,hr.employees e
where d.department_id = e.department_id
and d.department_name in ('IT','Sales')
GROUP BY d.department_name;
�Ż����飺 ����������
�Ż������� ��

* SELECT d.department_name,count(e.job_id)as "����������",
avg(e.salary)as "ƽ������"
FROM hr.departments d,hr.employees e
WHERE d.department_id = e.department_id
GROUP BY d.department_name
HAVING d.department_name in ('IT','Sales');


