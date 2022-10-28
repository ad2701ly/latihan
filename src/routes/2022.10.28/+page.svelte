<script lang="ts">
	const uangSaya = 20000;

	const hargaCilok = 5000;
	const hargaCakue = 1000;
	const hargaSate = 15000;

	let bisaBeliSate: string;
	let bisaBeliCilok: string;

	//pembuktian kondisi benar atau salah
	// "if" untuk pengecekan kondisi, jika benar, kode dalam "if" akan dieksekusi
	// jika salah kode dalam "else" akan dieksekusi
	if (uangSaya < hargaSate) {
		bisaBeliSate = 'Uang Anda Kurang Banyak untuk beli sate';
	} else {
		bisaBeliSate = 'Anda bisa Beli sate';
	}

	if (uangSaya < hargaCilok) {
		bisaBeliCilok = 'Uang Anda Kurang Banyak untuk beli cilok';
	} else {
		bisaBeliCilok = 'Anda bisa Beli cilok';
	}
</script>

<p>
	{bisaBeliSate}
</p>

<p>
	{bisaBeliCilok}
</p>
