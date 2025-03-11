Nama : Ischika Afrilla

NPM : 2306227955

Advance Programming - B
## Module 5 - Java Profiling
1. Test plan GUI for endpoints `/all-student-name`
   ![all-student-name-graph](image/all-student-name-graph.png)
   ![all-student-name-summary](image/all-student-name-summary.png)
   ![all-student-name-table](image/all-student-name-table.png)
   ![all-student-name-tree](image/all-student-name-tree.png)
2. Test plan GUI for endpoints `/highest-gpa`
   ![highest-gpa-graph](image/highest-gpa-graph.png)
   ![highest-gpa-summary](image/highest-gpa-summary.png)
   ![highest-gpa-table](image/highest-gpa-table.png)
   ![highest-gpa-tree](image/highest-gpa-tree.png)
3. Test plan command line for endpoints `/all-student-name`
   ![cmd-allstudname](image/cmd_allstudname.png)
   ![res-allstudname](image/res-allstudname.png)
4. Test plan command line for endpoints `/highest-gpa`
   ![cmd-gpa](image/cmd_gpa.png)
   ![res-gpa](image/res-highestgpa.png)

### After Refactoring
1. endpoints `/all-student`
![optimized-all-student](image/optimized-all-student.png)
2. endpoints `/all-student-name`
![optimized-all-student-name](image/optimized-all-student-name.png)
3. endpoints `/highest-gpa`
![optimized-gpa](image/optimized-gpa.png)

Berdasarkan data di atas, terlihat bahwa waktu eksekusi untuk endpoint `/all-student` mengalami penurunan lebih dari 20% pada sample time JMeter setelah dilakukannya refactoring. Penurunan signifikan juga terjadi pada endpoint `/all-student-name` dan `/highest-gpa`. Hal ini menunjukkan bahwa optimasi melalui refactoring fungsi memiliki dampak yang cukup besar terhadap nilai uji menggunakan JMeter.

### Reflection
1. What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?
   JMeter digunakan untuk menguji performa aplikasi dari sisi beban dan respons, mensimulasikan banyak pengguna sekaligus. Sementara itu, IntelliJ Profiler digunakan untuk menganalisis performa aplikasi di tingkat kode, membantu menemukan bottleneck seperti penggunaan CPU atau memori yang berlebihan.

2. How does the profiling process help you in identifying and understanding the weak points in your application?
   Profiling membantu mengidentifikasi bagian kode yang tidak efisien, seperti metode yang terlalu lambat atau konsumsi sumber daya yang tinggi, sehingga dapat dilakukan optimasi yang lebih spesifik.

3. Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?
   Ya, IntelliJ Profiler efektif dalam menganalisis bottleneck karena menyediakan informasi rinci tentang penggunaan CPU, memori, dan eksekusi metode, sehingga memudahkan pengembang dalam mengoptimalkan performa aplikasi.

4. What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?

5. What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?
   IntelliJ Profiler membantu menemukan bottleneck di level kode, memberikan wawasan tentang penggunaan CPU dan memori, serta memungkinkan optimasi yang lebih tepat pada bagian kode yang bermasalah.

6. How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter?
   Perbedaan hasil dapat terjadi karena JMeter menguji beban aplikasi secara keseluruhan, sedangkan Profiling lebih berfokus pada kode internal. Untuk mengatasinya, saya menganalisis hasil keduanya secara bersamaan dan menyesuaikan dengan konteks pengujian untuk mendapatkan solusi yang tepat.

7. What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?
