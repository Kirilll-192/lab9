#include "Stdafx.h"
using namespace std;

  void hard()
    {
        /*
         - подсчитать количество заявок на ремонт в прошлом году и отобразить информацию о них;
         - найти и отобразить информацию о самом длительном устранении неисправности в этом году с учетом даты
           и времени; - упорядочить исходную информацию по файлам, где в качестве имени файла используется год,
           в котором произошла поломка, а в качестве содержимого
         - сведения обо всех поломках за этот год.

       */
        cout << "\nHard task level: \n";
             time_t now = time(0);

   cout << "Number of sec since January 1,1970:" << now << endl;

   tm *ltm = localtime(&now);

   // print various components of tm structure.
   cout << "Year" << 1970 + ltm->tm_year<<endl;
   cout << "Month: "<< 1 + ltm->tm_mon<< endl;
   cout << "Day: "<<  ltm->tm_mday << endl;
   cout << "Time: "<< 1 + ltm->tm_hour << ":";
   cout << 1 + ltm->tm_min << ":";
   cout << 1 + ltm->tm_sec << endl;
    struct tm *u;
  char s1[40] = { 0 }, s2[40] = { 0 };
  const time_t timer = time(NULL);
  u = localtime(&timer);
  strftime(s1, 80, "%d.%m.%Y %H:%M:%S ", u);
  printf("%s\n", s1);
  u->tm_mday += ADD_DAYS;
  time_t next = mktime(u);
  u = localtime(&next);
  strftime(s2, 80, "%d.%m.%Y %H:%M:%S ", u);
  printf("%s\n", s2);
int count = 10;
	Book* mas_book = new Book[count];
	mas_book = FillStruct(mas_book, count);
	SaveFile(mas_book, count);
	mas_book = LoadFile(count);
	cout << "\nСодержимое файла до внесенных изминений: \n";
	cout << "\nВ файле хранится масив структур содержащих следущие поля: \n";
	cout << "\t-ФИО автора\n\t-название книги\n\t-цена за ед.\n\t-количетсво экзэмпляров";
	ShowBooks(mas_book, count);
	cout << "\nСодержимое файла после внесенных изминений: "
		 <<  "\nДанные про книги авторов, фамилия которых начинается с буквы “К”: \n";
	IsSetDiscount(count);
	Book* buffer = new Book[count];
	buffer = LoadFile(count);
	SaveFile(buffer, count);
	ShowBooks(buffer, count);
        cout << "\nНажмите <Enter> чтобы продолжить: ";
        while (getchar() != '\n')
            continue;
    }
