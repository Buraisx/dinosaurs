[See assignment in Alexa](https://alexa.bitmaker.co/cohorts/72/assignments/2247/latest)

SELECT COUNT(*) from dinos;

SELECT * FROM dinos WHERE period = 'Jurassic';

SELECT SUM(length) FROM dinos WHERE PERIOD = 'Cretaceous';

SELECT * FROM dinos WHERE PERIOD = 'Jurassic' OR PERIOD = 'Cretaceous' ORDER BY species ASC;

SELECT * FROM dinos WHERE t_order = 'Saurischia' and diet = 'Herbivorous';

UPDATE dinos SET name = 'shortie' WHERE length = (SELECT MIN(length) FROM dinos);
SELECT * FROM dinos WHERE length = (SELECT MIN(length) FROM dinos);

SELECT * FROM dinos ORDER BY name ASC LIMIT 1;