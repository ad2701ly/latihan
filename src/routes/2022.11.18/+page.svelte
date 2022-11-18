<script lang="ts">
	let hari: string = 'kamis';
	let hasil: string;

	//console.log untuk mengecek hasil (debug)
	//Huruf kecil dan besar berpengaruh
	if (hari == 'Jumat') {
		//console.log('Hari ini hari jumat');
		hasil = 'Hari Jumat';
	} else if (hari == 'Kamis') {
		//console.log('Hari ini hari kamis');
		hasil = 'hari kamis';
	} else {
		//console.log('Bukan Kamis dan Jumat');
		hasil = 'bukan kamis dan jumat';
	}

	//const masuk = window.prompt('Masukkan Nama Anda');
	// Tanda ! untuk mambalik nilai benar / salah saja,
	/* console.log(!masuk);
	if (!masuk) {
		window.history.back();
	} */

	const angka1 = 5;
	const angka2 = 5;
	let perbandingan = '';
	// '>' tanda lebih besar
	// '<' tanda lebih kecil
	if (angka1 > angka2) {
		//console.log(angka1 + ' lebih besar dari ' + angka2);
		perbandingan = angka1 + ' lebih besar dari ' + angka2;
	} else if (angka1 == angka2) {
		//console.log(angka1 + ' nilai yang sama ' + angka2);
		perbandingan = angka1 + ' nilai yang sama ' + angka2;
	} else {
		//console.log(angka1 + ' lebih kecil dari ' + angka2);
		perbandingan = angka1 + ' lebih kecil dari ' + angka2;
	}
	console.log(4 % 2);
</script>

<h1>Latihan Logika</h1>

<p>{hasil}</p>
<p>{perbandingan}</p>

<h1>Tugas</h1>
<p>angka 2 itu genap karena bisa dibagi 2</p>
<p>angka 5 itu ganjil tidak bisa dibagi 2</p>
