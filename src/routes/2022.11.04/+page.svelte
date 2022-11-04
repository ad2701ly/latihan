<script>
	// if(yang mau diuji){
	// jika benar kode akan dieksekusi
	//}else{
	//jika kondisi tidak seperti yang diharapkan
	//}

	let hari = new Date().getDay();
	let kegiatan = '';
	let namaHari = ['Minggu', 'Senin', 'Selasa', 'Rabu', 'Kamis', 'Jumat', 'Sabtu'];

	if (namaHari[hari] == 'Jumat') {
		kegiatan = 'Saya melakukan kegiatan Muroja ah pagi';
	} else if (namaHari[hari] == 'Senin') {
		kegiatan = 'Saya akan masuk sekolah';
	} else if (namaHari[hari] == 'Selasa') {
		kegiatan = 'Saya akan olahraga';
	} else {
		kegiatan = 'Saya masih merencanakan sesuatu';
	}

	let a = [20, 100, 22, 38, 40, 23];
	let b = [50, 50, 22, 59, 20, 45];
</script>

<p>{hari}</p>
<p>{namaHari[0]}</p>

<p>{kegiatan}</p>

<h1>Latihan</h1>
<table border={1}>
	<tr>
		<th>A</th>
		<th>B</th>
		<th>A>B</th>
		<th>A{`<`}B </th>
		<th>A=B</th>
	</tr>
	<tr>
		<td>{a[0]}</td>
		<td>{b[0]}</td>
		<td>{a[0] > b[0] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[0] < b[0] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[0] == b[0] ? 'BENAR' : 'SALAH'}</td>
	</tr>
	<tr>
		<td>{a[1]}</td>
		<td>{b[1]}</td>
		<td>{a[1] > b[1] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[1] < b[1] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[1] == b[1] ? 'BENAR' : 'SALAH'}</td>
	</tr>
	<tr>
		<td>{a[2]}</td>
		<td>{b[2]}</td>
		<td>{a[2] > b[2] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[2] < b[2] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[2] == b[2] ? 'BENAR' : 'SALAH'}</td>
	</tr>
	<tr>
		<td>{a[3]}</td>
		<td>{b[3]}</td>
		<td>{a[3] > b[3] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[3] < b[3] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[3] == b[3] ? 'BENAR' : 'SALAH'}</td>
	</tr>
	<tr>
		<td>{a[4]}</td>
		<td>{b[4]}</td>
		<td>{a[4] > b[4] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[4] < b[4] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[4] == b[4] ? 'BENAR' : 'SALAH'}</td>
	</tr>
	<tr>
		<td>{a[5]}</td>
		<td>{b[5]}</td>
		<td>{a[5] > b[5] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[5] < b[5] ? 'BENAR' : 'SALAH'}</td>
		<td>{a[5] == b[5] ? 'BENAR' : 'SALAH'}</td>
	</tr>
</table>

<style>
	table {
		width: 100%;
		border: solid black 1;
		max-width: 500px;
		margin: auto;
	}
	td {
		text-align: center;
	}
	th {
		background-color: red;
	}
</style>
