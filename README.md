# Program-C_TLS21
Rust_Galantandra Jabbarul Ahmad
//GALANTANDRA JABBARUL AHMAD 473878
#include <iostream>
#include <math.h>
using namespace std;

int main()
{
    int bangun;
    cout<<"#Selamat datang di kalkulator bangun datar dan bangun ruang#\n";
    cout<<"\n============================================================\n\n";
    cout<<"Pilih jenis bangun\n";
    cout<<"1 untuk Bangun Datar\n";
    cout<<"2 untuk Bangun Ruang\n";
    cout<<"Masukkan angka bangun yang diinginkan : ";
    cin>>bangun;
    cout<<"\n============================================================\n\n";
    switch(bangun)
    {
         case 1:
            int bangundatar;
            cout<<"Anda memilih bangun datar\n\n";
            cout<<"1 untuk Persegi\n";
            cout<<"2 untuk Persegi panjang\n";
            cout<<"3 untuk Lingkaran\n";
            cout<<"4 untuk Segitiga sama sisi\n";
            cout<<"5 untuk Layang-layang\n";
            cout<<"6 untuk Jajar Genjang\n";
            cout<<"7 untuk Trapesium sama kaki\n";
            cout<<"8 untuk Belah ketupat\n";
            cout<<"Masukkan angka bangun datar yang diinginkan : ";
            cin>>bangundatar;
            cout<<"\n============================================================\n\n";
            switch (bangundatar)
            {
                float s,p,l,K,L,pi,r,a,t,d1,d2,s_miring,s_atas,s_bawah;
                case 1:
                    cout<<"Persegi\n\n";
                    cout<<"Masukkan nilai s : ";
                    cin>>s;
                    K = 4*s;
                    L = s*s;
                    cout<<"Nilai keliling : "<<K<<endl;
                    cout<<"Nilai luas : "<<L<<endl;
                    break;

                case 2:
                    cout<<"Persegi Panjang\n\n";
                    cout<<"Masukkan nilai panjang : ";
                    cin>>p;
                    cout<<"Masukkan nilai lebar : ";
                    cin>>l;
                    K = (2*p)+(2*l);
                    L = p*l;
                    cout<<"Nilai keliling : "<<K<<endl;
                    cout<<"Nilai luas : "<<L<<endl;
                    break;

                case 3:
                    pi=3,14;
                    cout<<"Lingkaran\n\n";
                    cout<<"Masukkan nilai jari-jari : ";
                    cin>>r;
                    K = 2*pi*r;
                    L = pi*r*r;
                    cout<<"Nilai keliling : "<<K<<endl;
                    cout<<"Nilai luas : "<<L<<endl;
                    break;

                case 4:
                    cout<<"Segitiga sama sisi\n\n";
                    cout<<"Masukkan nilai alas : ";
                    cin>>a;
                    cout<<"Masukkan nilai tinggi : ";
                    cin>>t;
                    K = 3*a;
                    L = (1.0/2.0)*a*t;
                    cout<<"Nilai keliling : "<<K<<endl;
                    cout<<"Nilai luas : "<<L<<endl;
                    break;

                case 5:
                    cout<<"Layang-layang\n";
                    cout<<"Masukkan nilai diagonal 1 : ";
                    cin>>d1;
                    cout<<"Masukkan nilai diagonal 2 : ";
                    cin>>d2;
                    cout<<"Masukkan nilai sisi bawah : ";
                    cin>>s_bawah;
                    cout<<"Masukkan nilai sisi atas : ";
                    cin>>s_atas;
                    L = (1.0/2.0)*d1*d2;
                    K = (2*s_bawah)+(2*s_atas);
                    cout<<"Nilai keliling : "<<K<<endl;
                    cout<<"Nilai luas : "<<L<<endl;
                    break;

                case 6:
                    cout<<"Jajar Genjang\n";
                    cout<<"Masukkan nilai alas : ";
                    cin>>a;
                    cout<<"Masukkan nilai tinggi : ";
                    cin>>t;
                    cout<<"Masukkan nilai sisi miring : ";
                    cin>>s_miring;
                    L = a*t;
                    K = 2*(a+s_miring);
                    cout<<"Nilai keliling : "<<K<<endl;
                    cout<<"Nilai luas : "<<L<<endl;
                    break;

                case 7:
                    cout<<"Trapesium sama kaki\n";
                    cout<<"Masukkan nilai tinggi : ";
                    cin>>t;
                    cout<<"Masukkan nilai sisi atas : ";
                    cin>>s_atas;
                    cout<<"Masukkan nilai sisi bawah : ";
                    cin>>s_bawah;
                    cout<<"Masukkan nilai sisi miring : ";
                    cin>>s_miring;
                    L = (1.0/2.0)*(s_atas+s_bawah)*t;
                    K = s_atas+s_bawah+(2*s_miring);
                    cout<<"Nilai keliling : "<<K<<endl;
                    cout<<"Nilai luas : "<<L<<endl;
                    break;

                case 8:
                    cout<<"Belah ketupat\n";
                    cout<<"Masukkan nilai diagonal 1 : ";
                    cin>>d1;
                    cout<<"Masukkan nilai diagonal 2 : ";
                    cin>>d2;
                    cout<<"Masukkan nilai sisi bawah : ";
                    cin>>s_bawah;
                    cout<<"Masukkan nilai sisi atas : ";
                    cin>>s_atas;
                    L = (1.0/2.0)*d1*d2;
                    K = (2*s_bawah)+(2*s_atas);
                    cout<<"Nilai keliling : "<<K<<endl;
                    cout<<"Nilai luas : "<<L<<endl;
                    break;

                    default:
                    cout<<"Pilihan Anda salah!\n";
                    cout<<"Masukkan pilihan yang tepat, yaitu 1-8!\n";
            }
            break;
            case 2 :
                int bangunruang;
                cout<<"Anda memilih bangun ruang\n";
                cout<<"1 untuk Kubus\n";
                cout<<"2 untuk Balok\n";
                cout<<"3 untuk Tabung\n";
                cout<<"4 untuk Kerucut\n";
                cout<<"5 untuk Bola\n";
                cout<<"6 untuk Prisma segitiga\n";
                cout<<"7 untuk Limas segitiga\n";
                cout<<"8 untuk Limas segiempat\n";
                cout<<"Masukkan angka bangun yang diinginkan : ";
                cin>>bangunruang;
                cout<<"\n============================================================\n\n";
                switch (bangunruang)
                {
                    float d,t,r,V,A,pi,s,a,p,l,b;
                    case 1:
                        cout<<"Kubus\n\n";
                        cout<<"Masukkan nilai sisi : ";
                        cin>>s;
                        A = 6*s*s;
                        V = s*s*s;
                        cout<<"Nilai luas permukaan : "<<A<<endl;
                        cout<<"Nilai volume : "<<V<<endl;
                        break;

                    case 2:
                        cout<<"Balok\n\n";
                        cout<<"Masukkan nilai panjang : ";
                        cin>>p;
                        cout<<"Masukkan nilai lebar : ";
                        cin>>l;
                        cout<<"Masukkan nilai tinggi : ";
                        cin>>t;
                        A = 2*(p*l+p*t+l*t);
                        V = p*l*t;
                        cout<<"Nilai luas permukaan : "<<A<<endl;
                        cout<<"Nilai volume : "<<V<<endl;
                        break;

                    case 3:
                        cout<<"Tabung\n\n";
                        cout<<"Masukkan diameter : ";
                        cin>>d;
                        cout<<"Masukkan tinggi : ";
                        cin>>t;
                        pi = 3,14;
                        A  = (2 * pi * (d/2) * t) + (2 * pi * (d/2) * (d/2));
                        V  = pi * (d/2) * (d/2) * t;
                        cout<<"Nilai luas permukaan : "<<A<<endl;
                        cout<<"Nilai volume : "<<V<<endl;
                        break;

                    case 4:
                        cout<<"Kerucut\n\n";
                        cout<<"Masukkan diameter : ";
                        cin>>d;
                        cout<<"Masukkan tinggi : ";
                        cin>>t;
                        pi = 3.14;
                        A  = pi * (d/2) * ((d/2) + sqrt(((d * d) / 4) + (t * t)));
                        V  = (1.0/3.0) * pi * (d/2) * (d/2) * (t);
                        cout<<"Nilai luas permukaan : "<<A<<endl;
                        cout<<"Nilai volume : "<<V<<endl;
                        break;

                    case 5:
                        cout<<"Bola\n\n";
                        cout<<"Masukkan nilai jari-jari : ";
                        cin>>r;
                        pi = 3.14;
                        A  = 4*pi*r*r;
                        V  = (4.0/3.0)*pi*r*r*r;
                        cout<<"Nilai luas permukaan : "<<A<<endl;
                        cout<<"Nilai volume : "<<V<<endl;
                        break;

                    case 6:
                        cout<<"Prisma segitiga sama sisi\n\n";
                        cout<<"Masukkan nilai alas segitiga : ";
                        cin>>a;
                        cout<<"Masukkan nilai tinggi segitiga : ";
                        cin>>b;
                        cout<<"Masukkan nilai tinggi prisma : ";
                        cin>>t;
                        A = (a*b)+(3*a*t);
                        V = (1.0/2.0)*a*b*t;
                        cout<<"Nilai luas permukaan : "<<A<<endl;
                        cout<<"Nilai volume : "<<V<<endl;
                        break;

                    case 7:
                        cout<<"Limas segitiga sama sisi\n\n";
                        cout<<"Masukkan nilai alas segitiga : ";
                        cin>>a;
                        cout<<"Masukkan nilai tinggi segitiga : ";
                        cin>>b;
                        cout<<"Masukkan nilai tinggi prisma : ";
                        cin>>t;
                        A = ((1.0/2.0)*a*b)+(3*((1.0/2.0)*a*t));
                        V = (1.0/3.0)*(1.0/2.0)*a*b*t;
                        cout<<"Nilai luas permukaan : "<<A<<endl;
                        cout<<"Nilai volume : "<<V<<endl;
                        break;

                    case 8:
                        cout<<"Limas segiempat\n\n";
                        cout<<"Masukkan nilai panjang sisi alas : ";
                        cin>>p;
                        cout<<"Masukkan nilai lebar sisi alas : ";
                        cin>>l;
                        cout<<"Masukkan nilai tinggi limas : ";
                        cin>>t;
                        A = (p*l)+(p*t)+(l*t);
                        V = (1.0/3.0)*p*l*t;
                        cout<<"Nilai luas permukaan : "<<A<<endl;
                        cout<<"Nilai volume : "<<V<<endl;
                        break;

                    default:
                        cout<<"Pilihan Anda salah!\n";
                        cout<<"Masukkan pilihan yang tepat, yaitu 1-8!\n";
                }
    break;
    default:
        cout<<"Pilihan Anda salah!\n";
        cout<<"Masukkan pilihan yang tepat, yaitu 1 atau 2!\n";
    }
    return 0;
}
