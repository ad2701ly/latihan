<script lang="ts">
	//Pengenalan let dan const
	//let bisa diubah nilainya
	let angka = 45; //angka / number
	let desimal = 3.14;
	let huruf = 'huruf'; // string / huruf
	let pembenaran = false; // booleean / pembenaran

	//const tidak bisa diubah nilainya
	const lainnya = 'tak ubah';

	//mengganti variable / let
	angka = 20;
	huruf = 'contoh';
	huruf = 'Ganti';

	//Tipe data object
	let flashdisk = {
		merk: 'sandisk',
		ukuran: '16 GB',
		warma: 'merah dan hitam'
	};

	//tipe data array
	const warna = ['merah', 'biru', 'putih', 'ungu'];
</script>

<p>Angka : {angka}</p>
<p>Angka : {desimal}</p>
<p>Huruf :{huruf}</p>
<p>Pembenaran:{pembenaran}</p>

<p>{lainnya}</p>

<p>{flashdisk.ukuran}</p>
<p>{flashdisk.warma}</p>

<p>{warna}</p>
