#include <stdio.h>
#include <string.h>

int main() {
    float keiritan_pertamax_konstan = 15.0;
    float keiritan_pertamax_stopgo = 10.0;
    float keiritan_pertalite_konstan = 12.0;
    float keiritan_pertalite_stopgo = 8.0;

    float liter_bensin;
    char jenis_bensin[20];
    float jarak_tempuh;
    char mode_menyopir[20];
    
    printf("\n======================================================");
    printf("\n============== Simulasi Menyopir Mobil ===============");
    printf("\n======================================================\n");

    printf("\nMasukkan jumlah bensin  (liter)             : ");
    scanf("%f", &liter_bensin);
    printf("Masukkan jenis bensin   (pertamax/pertalite): ");
    scanf("%s", jenis_bensin);
    printf("Masukkan jarak tempuh   (KM)                : ");
    scanf("%f", &jarak_tempuh);
    printf("Masukkan mode menyopir  (konstan/stop&go)   : ");
    scanf("%s", mode_menyopir);

    float keiritan;

    if (strcmp(jenis_bensin, "pertamax") == 0) {
        if (strcmp(mode_menyopir, "konstan") == 0) {
            keiritan = keiritan_pertamax_konstan;
        } else if (strcmp(mode_menyopir, "stop&go") == 0) {
            keiritan = keiritan_pertamax_stopgo;
        } else {
            printf("Maaf, Mode menyopir tidak valid!\n");
        printf("\n======================================================\n");

            return 1;
        }
    } else if (strcmp(jenis_bensin, "pertalite") == 0) {
        if (strcmp(mode_menyopir, "konstan") == 0) {
            keiritan = keiritan_pertalite_konstan;
        } else if (strcmp(mode_menyopir, "stop&go") == 0) {
            keiritan = keiritan_pertalite_stopgo;
        } else {
            printf("Maaf, Mode menyopir tidak valid!\n");
        printf("\n======================================================\n");

            return 1;
        }
    } else {
        printf("\nMaaf, Jenis bensin tidak valid!\n");
        printf("\n======================================================\n");

        return 1;
    }

    float bensin_terpakai = jarak_tempuh / keiritan;
    float bensin_akhir = liter_bensin - bensin_terpakai;

    if (bensin_akhir < 0) {
        printf("\nHati-hati, Bensin akan habis sebelum sampai tujuan!\n");
        printf("\n======================================================\n");

    return 1;
}

    printf("\n=================== Hasil Simulasi ===================\n");
    printf("\n======================================================\n");
    printf("\nJumlah bensin yang terpakai                 : %.2f liter\n", bensin_terpakai);
    printf("Jumlah bensin yang tersisa                  : %.2f liter\n", bensin_akhir);
    printf("\n======================================================\n");

    return 0;
}
