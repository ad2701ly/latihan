<script lang="ts">
	let angka1 = 0,
		angka2 = 0;
</script>

<halaman>
	<div>
		<label for="">Angka 1</label>
		<input type="number" bind:value={angka1} />
	</div>
	<div>
		<label for="">Angka 2</label>
		<input type="number" bind:value={angka2} />
	</div>

	<p>
		<b>{angka1}</b> dan <b>{angka2}</b> adalah angka
		<b>{angka1 == angka2 ? 'Sama' : 'Beda'}</b>
	</p>

	<p>
		<b>{angka1}</b> Lebih <b>{angka1 >= angka2 ? 'Besar' : 'Kecil'}</b> dari <b>{angka2}</b>
	</p>
</halaman>

<style>
	halaman {
		display: flex;
		flex-direction: column;
		gap: 1rem;
		padding: 10px;
		min-height: 100%;
	}
</style>
