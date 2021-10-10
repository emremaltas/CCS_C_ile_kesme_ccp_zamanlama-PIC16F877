Bu projede şu ana kadar öğrendiğim Timer1,Timer2,B0 harici kesmesi ,B4-7 değişim kesmeleri ,CCP üzerinde durulmuştur ve devre haline getirilmiştir.

Devrede Neler OLuyor?

Sayac arttır butonuna basıldığında B0 ve C2 pinlerine lojik 1 girdisi verilmektedir. B0 harici kesme oluşturmakta ve displaydeki değer 1 artmaktadır. CCP1 yani C2 pini 4 kez lojik 1 yapıldığında yakalama gerçekleştiricek şekilde ayarlanmıştır ve yakalama meydana geldiğinde B1 pinindeki led yanmaktadır.

Timer 2 sayıcı olarak kullanılmıştır ve her T2 kesmesinde B2 pinindeki led toggle yapılmıştır.

Timer 1 zamanlayıcı olarak kullanılmış ve her kesmede CCP2 ucuna lojik 1 verilmiştir.CCP2 10 kez aktif olduğunda C3,20 kez olduğunda C4,30 kez olduğunda C5,40 kez olduğunda C6 pinlerindeki ledler yanmaktadır.Bu yanan led ile B4-B7 pinlerine kablo çekilmiştir ve B4-B7 kesmeleri meydana getirilmiştir.B4-B7 kesmelerinden hangisi meydana gelmiş ise 74ls164 entegresinden çıkış verilerek ledler ile o pinin değeri yansıtılmıştır.E0'a bağlı butona basıldığında Timer1,CCP2 kesmeleri ve sayac değeri LCD ekranında gösterilmiştir.

C7 pinine bağlı buton basıldığında ise tüm bu değerler sıfırlanmaktadır.Tüm bu kesmeler ve yapılan işlemler o an LCD ekranında da yazılarak bilgisi verilmiştir.

//Süre hesapları yapılmıştır ama burada değinilmemiştir!! //Fazla detay verilmeden yazılmıştır!!