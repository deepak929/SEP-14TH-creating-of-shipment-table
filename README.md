# SEP-14TH-creating-of-shipment-table
assignment done by me of vreating 6 tables of shipment




create table employee(
  EmplyoeeID INT UNSIGNED PRIMARY KEY,
  name VARCHAR (100)NOT NUL,
  Position VARCHAR(50) not null,
  salary DECIMAL(10,2) NOT NULL,
  Remarks TEXT NOT NULL
  );
  CREATE TABLE PALNET(
  PlanetID UNSIGNED PRIMARY KEY,
  Name  VARCHAR(100) NOT NULL,
  COORDINATES DOUBLE NOT NULL
  );
  CERATE TABLE SHIPMENT (
  SHIPMENTID INT UNSIGNED PRIMARY KEY,
  shipment DATE NOT NULL,
  managewr OT NULL,
  PLANET NOT NULL,
  FPREIGN KEY(manager) REFERENCE employee(ID),
  FOREIGN KEY(planet) REFERENCES PLANET(PLANETID),
  );
  CERATE TABLE has clearance
  (
  employee INT UNSIGNED ,
  PLANET INT UNSIGNED NOT NULL,
  LEVEL INT UNSIGNED NOT NULL,
  PRIMARY KEY (employee,planet),
  FOREIGN KEY (employee REFERENCES employee employeeID),
  fOREGIN KEY planet references ()
  );
  
  
  
  CREATE TABLE client
  (
  Account number INT UNSIGNED NOT NULL,
  name VARCHAR(30),
  PRIMARY KEY account number REFERENCES account numberID
  );
  CREATE TABLE package
  (
  shipment INT UNSIGNED NOT NULL ,
  package number INT UNSIGNED NOT NULL,
  contents VARCHAR,
  weight decimal(10,2),
  sender INT(30),
  Receptient INT UNSIGNED NOT NULL,
  PRIMARY KEY (shipment,package number),
  FOREIGN KEY (shipent REFERENCES shipmentID,sender REFERENCES senderID ,receptient REFERENCES receptientID),
  );
  
  
  
  
