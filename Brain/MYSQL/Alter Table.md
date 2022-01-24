### Alter Table

To add new column to an existing table, you use ALTER TABLE `ADD COLUMN` statement:

	ALTER TABLE table
	ADD [COLUMN] column_name column_definition [FIRST|AFTER existing_column];

- MySQL allows you to add the new column as the first column of the table by specifying the `FIRST` keyword. It also allows you to add the new column after an existing column using the `AFTER existing_column` clause. If you don’t explicitly specify the position of the new column, MySQL will add it as the last column.	

	