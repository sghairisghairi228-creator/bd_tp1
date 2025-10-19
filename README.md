**_### EXERCICE 1_**:

1/SQL> desc departement;  SELECT * FROM departement;
2/SQL>desc employees; SELECT* FROM employees;
3/SELECT * DESTINCT FROM employees;
4/SQL> SELECT employees_id as"EMP#",laste_name as "employe",job_id as "job",hire_date as "HIRE DATE FROM employees;
5/ SELECT First_name,employes,job_id as "employes and title" FROM employees;

**_### EXERCICE 2_**:
1/SELECT last_name,SALARY FROM employees WHERE SALARY>12000;
2/ SELECT last_name,Departement_ID FROM employees WHERE Departement_ID="176";
3/SELECT last_name,SALARY FROM employees WHERE SALARY NOT BETWEEN(5000 AND 12000);
4/SELECT last_name,job_id,HIRE_DATE FROM employees WHERE last_name="matos" AND last_name="taylor" ORDER BY HIRE_DATE ASC;
5/SELECT last_name ,departemet_id FROM employees WHERE departement_id=20 AND departement_id=50 ORDER BY last_name ASC;
6/SELECT last_name , first_ name FROM EMPLOYEES WHERE SALARY BETWEEN(5000 AND 12000) AND Departement_id=20 OR departement_id=50;
7/SELECT last_name , job_id FROM employees WHERE Manager_id isNULL;
8/SELECT last_name , SALARY ,commission_pct FROM employees WHERE commission_pct is NOT NULL;
9/SELECT last_name FROM employees WHERE last_name="--a";
10/ SELECT * FROM employees WHERE last_name LIKE %a AND last_name LIKE %e;
11/SELECT last_name,SALARY,Commission_pct FROM employees WHERE commission_pct="20%";


**_### EXERCICE 2_**:
`1/SELECT employee_id , last_name,SALARY +15.5% as NEW_SALARY FROM employees;
2/SELECT employee_id , last_name,SALARY +15%,SALARY +15.5% as NEW_SALARY FROM employees;

3/SELECT last_name LENGTH(last_name) FROM employees WHERE last_name LIKE  ' %j' OR last_name LIKE'  %A' OR last_name LIKE '%M'
4/SELECT last_name ,LPAD(TO_CHAR(SALARY),15,'$') FROM employees;
5/SELECT last_name , NVL(TO_CHAR(commission_pct),'NO COMMISSION') FROM employees;
6/ SELECT NEXT_DAY(date_embauche,'MONDAY') FROM employees;
7/SELECT date_embauche , TRUNC(date_embauche ,'YEAR') FROM employees;
8/SELECT date_embauche ,TRUNC(SYSDATE) - TRUNC(date_embauche) FROM employees;
