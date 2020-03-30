# soal bigdata
1. Cari dan sebutkan 3 DBMS yang bisa digunakan untuk mengelola big data
2. Carilah contoh masalah big data yang bisa dikelola menggunakan salah satu DBMS tersebut, jelaskan mulai dari instalasi sampai CRUD untuk data menggunakan DBMS tersebut. Asumsikan anda akan memecahkan masalah big data yang sudah anda cari contoh tadi, jelaskan kira-kira bagaimana arsitektur dari solusi big data menggunakan DBMS tersebut, gambarkan diagramnya.

# Jawaban 

1. -Mongodb -Cassandra -Neo4j
2. Disini saya memilih neo4j, merupakan jenis graph database, dimana nanti bentuknya berupa2 node yang saling terhubung satu dengan lainnnya sesuai relasi yang dimiliki. Dalam kasus big data ambil saja contoh relasi antara 1 orang dengan orang lain yang bisa berupa ayah, ibu, saudara, teman dll.
Untuk melakukan instalasi saya menggunakan ubuntu. Masuk ke terminal dan install terlebih dahulu neo4j dengan menjalankan perintah berikut:
sudo apt-get install -y neo4j
jika sudah terinstall maka jalankan neo4j dengan perintah:
sudo neo4j start
jika sudah maka buka localhost pada browser untuk menjalankannya.

Disini akan dibuat beberapa contoh node yang diperlukan. Diantaranya membuat nama2 orang dan kaitannya dengan orang lain. Gunakan cypher query.

CREATE (Joko:Person {name:"Joko Tingkir", born:1991})
