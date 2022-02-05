#include<stdio.h>
int main(){
int final,vize,odev,sonuc;
float ort;
printf("vize notunuzu giriniz");
scanf("%d",&vize);
printf("odev notunuzu giriniz");
scanf("%d",&odev);
printf("final notunuzu giriniz");
scanf("%d",&final);
printf("ortalamanizi giriniz");
scanf("%f",&ort);

sonuc=((odev*40/100+vize*60/100)+final)/2;

if(sonuc<0 ||sonuc>100 || ort<0 || ort>4)
printf("gecersiz bir not veya ortalama girdiniz");
return 0;
if(sonuc>=90)
printf("ders harf notunuz: AA");
else if (sonuc>=80)
printf("ders harf notunuz: BA");
else if (sonuc>=70)
printf("ders harf notunuz: BB");
else if (sonuc>=65)
printf("ders harf notunuz: CB");
else if (sonuc>=60)
printf("ders harf notunuz: CC");
else if (sonuc>=55){
printf("ders harf notunuz: DC");
if (ort>3.0)
printf("\nortalaman yuksek oldugu icin dersten gectin");
else printf("\nkaldiniz");
}
else if (sonuc>=50){
printf("ders harf notunuz: DD");
if (ort>=3.7)
printf("\nortalaman yuksek oldugu icin dersten gectin");
else printf("\nkaldiniz");
}
else if (sonuc>=45)
printf("ders harf notunuz: FD\n bute kaldin ");
else if (sonuc<45)
printf("ders harf notunuz: FF\n dersten her turlu kaldiniz");
return 0;
}
