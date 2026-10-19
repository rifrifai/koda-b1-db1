```mermaid
	erDiagram

	Buku }|--|| Peminjam : Borrowed
	Buku }|--|| Kategori : Contains
	Kategori ||--|| Rak_Buku : Contains
	Rak_Buku ||--|{ Buku : Contains
	Petugas ||--|{ Peminjam : Set

	Buku {
		int id_buku
		string nama_buku
		string penulis
		int jumlah
	}

	Kategori {
		int id_kategori
		string nama_kategori
	}

	Rak_Buku {
		int id_rak
		string nama_rak
	}

	Petugas {
		int id_petugas
		string nama_petugas
	}

	Peminjam {
		int id_peminjam
		string nama_peminjam
	}

```