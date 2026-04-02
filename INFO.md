# Base de donnée :
Nom de projet : Crousty Movies
MDP : CroustyLover92I
DATABASE_URL=postgresql://postgres.zpdugyojedzybursowrc:CroustyLover92I@aws-1-eu-west-3.pooler.supabase.com:5432/postgres

host: aws-1-eu-west-3.pooler.supabase.com
port: 5432
database: postgres
user: postgres.zpdugyojedzybursowrc



extension=pdo_pgsql
extension=pgsql

# Template d'ajout

INSERT INTO film (titre, annee, duree, resume, affiche, bandeAnnonce, realisateur, acteurs, idGenre) VALUES 
(
    'Inception', 
    2010, 
    148, 
    'Un voleur qui subtilise des secrets par le biais du rêve.', 
    'https://lien-image.com/inception.jpg', 
    'https://youtube.com/v=xxx', 
    'Christopher Nolan', 
    'Leonardo DiCaprio, Elliot Page', 
    1 -- 1 correspond ici à Science-Fiction
);

INSERT INTO commentaire (note, pseudo, avis, idFilm) VALUES 
(5, 'Crousty', 'Incroyable, un chef d’oeuvre !', 1),
(4, 'User123', 'Un peu complexe mais super visuels.', 1),
(5, 'BatmanFan', 'Le meilleur film de super-héros.', 2);

INSERT INTO genre (libelle) VALUES 
('Science-Fiction'),
('Action'),
('Drame'),
('Comédie'),
('Horreur');