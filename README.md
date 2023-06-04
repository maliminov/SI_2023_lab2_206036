# Втора лабораториска вежба по Софтверско инженерство
## Миле Малиминов, бр. на индекс 206036

>2) Control Flow Graph (CFG)

![Control Flow Graph](https://github.com/maliminov/SI_2023_lab2_206036/assets/130310740/86bd64a8-5b05-4587-a9d8-e5aaf7a0c900)


>3) Цикломатска комплексност

Цикломатската комплексност на овој код е 11, истата ја добив преку формулата M = E - N + 2: каде што E е бројот на ребра, а N е бројот на јазли. Па, имаме M = 33 - 24 + 2 = 11. Значи, цикломатската комплексност изнесува 11.


>4) Тест случаи според критериумот Every Branch

1. Тест за условот за RuntimeException
2. Тест за условот за празен username при што се доделува мејлот
3. Тест за валидноста на внесениот мејл
4. Тест за содржење на username-от во password-ot, или дали истиот е пократок од 8 
5. Тест за празно место во password-от
6. Тест за содржење на специјални знаци во password-ot

>5) Тест случаи според критериумот Multiple Condition за условот *if (user==null || user.getPassword()==null || user.getEmail()==null)*

1. (T,X,X) - кога user-от е null, а password и email може да се anything / што било

2. (F,T,X) - user!=null, null password, email anything

3. (F,F,T) - user!=null, password!=null, null email 

4. (F,F,F) - user, password и email сите не се null, и се избегнува RuntimeException.
