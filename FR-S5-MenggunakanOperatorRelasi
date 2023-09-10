#include <stdio.h>

int main() {
    char nama[50];
    char nim[20];
    float nilai_tugas, nilai_uts, nilai_uas, nilai_akhir;
    char grade;
    
    printf("\n============================================");
    printf("\n======== Penilaian Mahasiswa Cemara ========");
    printf("\n============================================\n");

    // Input
    printf("Nama            : ");
    fgets(nama, sizeof(nama), stdin);
    printf("NIM             : ");
    fgets(nim, sizeof(nim), stdin);

    printf("Nilai Tugas     : ");
    if (scanf("%f", &nilai_tugas) != 1 || nilai_tugas < 0 || nilai_tugas > 100) {
        printf("Nilai Tugas tidak valid.\n");
        return 1;
    }

    printf("Nilai UTS       : ");
    if (scanf("%f", &nilai_uts) != 1 || nilai_uts < 0 || nilai_uts > 100) {
        printf("Nilai UTS tidak valid.\n");
        return 1;
    }

    printf("Nilai UAS       : ");
    if (scanf("%f", &nilai_uas) != 1 || nilai_uas < 0 || nilai_uas > 100) {
        printf("Nilai UAS tidak valid.\n");
        return 1;
    }

    // Menghitung Nilai Akhir
    nilai_akhir = (0.4 * nilai_tugas) + (0.3 * nilai_uts) + (0.3 * nilai_uas);

    // Menentukan Grade
    if (nilai_akhir >= 90) {
        grade = 'A';
    } else if (nilai_akhir >= 85) {
        grade = 'A';
    } else if (nilai_akhir >= 80) {
        grade = 'B';
    } else if (nilai_akhir >= 75) {
        grade = 'B';
    } else if (nilai_akhir >= 70) {
        grade = 'B';
    } else if (nilai_akhir >= 65) {
        grade = 'C';
    } else if (nilai_akhir >= 50) {
        grade = 'D';
    } else {
        grade = 'E';
    }

    // Output
    printf("\n============= Hasil Penilaian ==============");
    printf("\nNama            : %s", nama);
    printf("NIM             : %s", nim);
    printf("Nilai Akhir     : %.2f\n", nilai_akhir);
    printf("Grade           : %c\n", grade);
    printf("\n============================================\n");

    return 0;
}
