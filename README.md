# jfsdexam
CREATE DATABASE labexam;

USE labexam;

CREATE TABLE customers (
    id BIGINT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL UNIQUE,
    phone VARCHAR(15) NOT NULL UNIQUE,
    address VARCHAR(255),
    date_of_birth DATE
);

INSERT INTO customers (name, email, phone, address, date_of_birth)
VALUES 
('John Doe', 'john.doe@example.com', '1234567890', '123 Elm St', '1990-05-15'),
('Jane Smith', 'jane.smith@example.com', '9876543210', '456 Oak St', '1995-07-20');
