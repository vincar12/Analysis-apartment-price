# Analisis Harga Apartemen

### 1. Project Overview
Tujuan dari proyek ini adalah untuk membuat analisa harga apartemen di Amerika Serikat dengan visualisasi dan dashboard untuk menarik insight bisnis.

---

### 2. Project Structure
```bash
├── h8dsft_Milestone1_Vincar.ipynb           # Jupyter notebook untuk analisis dan pembuatan model
├── apartments_for_rent_classified_10K.csv   # Dataset asli
├── README.md                                # Project README file
```

---

### 3. Workflow
1. **Data Loading**:
   - Data dimuat dalam pandas dataframe dari csv.
   
2. **Data Cleaning**:
   - Membersihkan nilai-nilai null, encoding beberapa kolom, serta ubah data type.

4. **Analysis**:
   - **Handling Outlier**: Handling data *outlier* dengan menghitung skew dan menggunakan *Z-Score* atau *Tukey's Rule*; lalu dilakukan *capping* dengan *winsorizer*
   - **Visualization**: Menampilkan visualisasi untuk analisis data apartemen.
     
5. **Kesimpulan & Rekomendasi**:
   - Berisi kesimpulan dari proyek ini serta rekomendasi bisnis berdasarkan model yang dibuat.

---

### 4. Hasil dan Kesimpulan

[Tableau Dashboard](https://public.tableau.com/views/Milestone1_17200887994370/Dashboard2?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

Berdasarkan eksplorasi, cleaning, dan analisis data listing apartemen dapat disimpulkan beberapa informasi terkait data apartemen;
1. Terlihat bahwa luas rata-rata apartemen memiliki rentang yang cukup jauh antar state. Dari yang terbesar West Virginia 1581.66 sqft, hingga yang terkecil District of Columbia dengan 537.37 sqft.
2. Persebaran jumlah unit apartemen pun rentangnya sangat besar; Texas yang memiliki nilai terbesar 1709 terpaut sangat jauh dengan Wyoming yang hanya memiliki 1 unit apartemen yang disewakan.
3. Sedangkan pada segi persentase aturan peliharaan, terbagi cukup rata antara 53,1% yang memperbolehkan baik anjing maupun kucing dan 40,9% yang melarang.
4. Harga apartemen memiliki persebaran yang terlihat sangat jauh, rata-rata apartemen dengan harga tertinggi berada dalam state Hawaii sebesar $2046,5 dan terendah pada state Wyoming dengan nilai $713.
5. Terdapat perbedaan signifikan secara statistik antara rata-rata harga apartemen di New Jersey dengan New York.
6. Faktor yang mempengaruhi harga unit diuji dengan analisa korelasi pearson test. Kolom yang memiliki korelasi signifikan dengan kolom harga dari test tersebut adalah:
    - square_feet yaitu luas unit apartemen
    - bathrooms yaitu jumlah kamar mandi
    - bedrooms yaitu jumlah kamar tidur.

Berdasarkan kesimpulan di atas, rekomendasi yang dapat diberikan untuk meningkatkan penjualan unit apartemen adalah sebagai berikut:
- Membuat apartemen dengan berbagai tipe seperti studio, 1 bedroom, 2 bedroom, dst. untuk menjangkau market yang besar.
- Meningkatkan promosi dengan mencantumkan foto-foto unit yang memikat pelanggan.
- Memastikan lokasi apartemen berada di daerah metropolitan atau justru kota satelit dapat lebih menguntungkan agar sesuai dengan pasar perantau yang butuh tempat tinggal.

---

### 5. References
- Dataset: [Apartment for Rent](https://archive.ics.uci.edu/dataset/555/apartment+for+rent+classified)
- Tools: Python, Pandas, NumPy, Seaborn, Matplotlib, Plotly, Scipy.
