### Foreign Key

	CREATE TABLE IF NOT EXISTS menu_banner(
		id INT AUTO_INCREMENT PRIMARY KEY,
		situacao INT(1),
	    title VARCHAR(255),
	    link VARCHAR(255),
	    image VARCHAR(255)
		tipoID int(1),
		PRIMARY KEY (id),  
		FOREIGN KEY (tipoID) REFERENCES tipo_banner_topo(id)
	);

