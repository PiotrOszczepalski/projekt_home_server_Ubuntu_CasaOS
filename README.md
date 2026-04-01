1) Podstawowy serwis komputera Dell i przygotowanie go do dalszej pracy:
   - wyczyszczenie starej pasty termoprzewodzącej z procesora i chłodzenia za pomocą alkoholu izopropylowego
   - nałożenie świeżej pasty na procesor
   - wyczyszczenie chłodzenia za pomocą sprężonego powietrza
   - wyczyszczenie płyty głównej szczotką antystatyczną
   - wyczyszczenie całego komputera z kurzu za pomocą sprężonego powietrza
   - ponowny montaż chłodzenia
   - podpięcie 2 dysków (SSD i HDD)

   ![01_chłodzenie](https://github.com/user-attachments/assets/5da78ce1-a3a5-4deb-9c56-3bf962972a0d)

   ![02_procesor](https://github.com/user-attachments/assets/f4453f44-2182-4a57-b0dd-a8f85fa88d7f)

   ![03_ipa](https://github.com/user-attachments/assets/0babdc06-7e53-49f0-a92b-a8dbc318fc9b)

   ![04_czyszczenie_procesora](https://github.com/user-attachments/assets/92ca5e44-dc5b-4f18-8bc8-63839f37979f)

   ![05_nowa_pasta](https://github.com/user-attachments/assets/808fa73e-42c6-4510-9218-793ea934a03d)

   ![06_czyszczenie_chłodzenia](https://github.com/user-attachments/assets/d53b45da-9fe9-4877-b4d0-93725084baad)

   ![07_czyste_chłodzenie](https://github.com/user-attachments/assets/83f2b335-8826-484e-a781-32182bbbc8e4)

   ![08_chłodzenie_powietrze](https://github.com/user-attachments/assets/724ec50c-2a4a-4870-9253-ac5513f4dd8d)

   ![09_czyszczenie_płyta](https://github.com/user-attachments/assets/592d3f3a-ea3d-4a6f-b1dc-d4107a0189f0)

   ![10_montaż_chłodzenia](https://github.com/user-attachments/assets/966301a1-deab-4170-810c-c0ecf05ba176)

   ![11_sprężone_powietrze](https://github.com/user-attachments/assets/dd0fcc21-06e3-4418-9af9-1fa84fdc936f)

   ![12_montaż_dysk_ssd](https://github.com/user-attachments/assets/e6981186-51df-487c-bc44-263349719544)

   ![13_montaż_dysk_hdd](https://github.com/user-attachments/assets/82810b80-9b2a-4b85-b99f-8eef8465d086)

2) Przygotowanie pendrive'a z systemem Linux Ubuntu Server za pomocą programu Rufus:

   ![14_rufus](https://github.com/user-attachments/assets/6ec1a59e-ddca-433c-a766-c9d450cb426b)

3) Instalacja systemu Linux Ubuntu Server:
   - podpięcie serwera do routera, aby uzyskał od niego adres ip i dostęp do internetu podczas instalacji
   - podpięcie pendrive'a z systemem
   - wybór języka
   - konfiguracja dysków (SSD na system oraz HDD na dane)
   - instalacja SSH
   - system zainstalowany
   - sprawdzenie, czy dyski są widoczne w systemie

   ![15_ethernet](https://github.com/user-attachments/assets/6690a49a-2475-40e5-812d-d22780fcf3ef)

   ![16_router](https://github.com/user-attachments/assets/2e21f41c-a1aa-4add-b7d7-dd3d5dbb2b94)

   ![17_pendrive](https://github.com/user-attachments/assets/065c9947-25e4-4268-9df0-0b4405c32d62)

   ![18_język](https://github.com/user-attachments/assets/335a07ac-c2dd-4b6a-a906-b936c08d6548)

   ![19_dysk1](https://github.com/user-attachments/assets/c1dc9d20-a7ef-43a1-9a67-999e4307e213)

   ![20_dysk2](https://github.com/user-attachments/assets/bbf3a43a-cd24-4227-9d73-6f39da63179a)

   ![21_wszystkie_dyski](https://github.com/user-attachments/assets/06766103-c76c-4034-a64d-96964b37fc74)

   ![22_ssh](https://github.com/user-attachments/assets/c8eaad65-bddf-418d-b8bb-a450b252ec14)

   ![23_instalacja](https://github.com/user-attachments/assets/15e2d8da-aa9c-4dd9-b3b1-324577675a3d)

   ![24_instalacja_gotowa](https://github.com/user-attachments/assets/4813252e-a715-43a1-8868-1e5d469bbfba)

   ![25_dyski_check](https://github.com/user-attachments/assets/109bc9be-5942-49d5-9135-3cd2b4d550de)

4) Ustawienie statycznego adresu ip dla serwera na routerze:

   ![26_statyczne_ip](https://github.com/user-attachments/assets/3a47e019-b8ac-4763-bbca-4e0190d5719e)

5) Konfiguracja SSH:
   - włączenie usługi SSH
   - włączenie automatycznego uruchamiania usługi serwera SSH podczas startu systemu
   - ponowne uruchomienie serwera, usługa SSH jest aktywna

   ![27_ssh](https://github.com/user-attachments/assets/338a6846-8843-4151-96ba-fae34770f467)

   ![28_ssh2](https://github.com/user-attachments/assets/7555fa78-f5a4-4d94-a5e2-67a5f15dc461)

6) Usługa SSH:
   - połączenie się z serwerem na komputerze będącym w tej samej sieci lokalnej
   - instalacja CasaOS
   - tworzenie konta
   - dostęp do panelu administracyjnego serwera

   ![29_ssh_logowanie](https://github.com/user-attachments/assets/5d83b5a7-1dd1-4b06-829c-b230e09b1378)
   
   ![30_casa_os_instalacja](https://github.com/user-attachments/assets/6dfad0e4-c12b-44ee-adc1-5c279976e7cd)

   ![31_casa_os_instalacja2](https://github.com/user-attachments/assets/70b354d1-518d-4f67-9d95-81a306c8dfa1)

   ![32_casa_os_tworzenie_konta](https://github.com/user-attachments/assets/baf73153-2386-4182-8261-4ff1d15738ce)

   ![33_casa_os_panel](https://github.com/user-attachments/assets/e48211b7-f3f5-40ae-9d42-372af342e7c5)

7) SAMBA:
   - konfiguracja udostępniania plików w sieci lokalnej przy użyciu protokołu SMB
   - udostępnienie katalogu sieciowego dostępnego z poziomu systemu Windows
   - transfer plików między hostem Windows a serwerem Linux

   ![34_nowy_folder_na_serwerze](https://github.com/user-attachments/assets/3ab0beab-af2e-4b4c-a8b7-de3b198cefba)
   
   ![35_skopiowanie_ścieżki](https://github.com/user-attachments/assets/52484c0f-5f8f-4528-bcbf-8bb25e5b2b61)

   ![36_eksplorator](https://github.com/user-attachments/assets/dd70d5a1-31f6-470e-a489-c0b200575e8b)

   ![37_upload_plików](https://github.com/user-attachments/assets/7a901e09-c85e-4568-a632-6cebf98a65df)

   ![38_pliki_na_serwerze](https://github.com/user-attachments/assets/2a770bca-626a-4623-bdd8-2d39fc81cece)

8) Wdrożenie usługi Jellyfin (streaming multimediów):
   - zainstalowanie Jellyfin na serwerze
   - wrzucenie filmów na serwer
   - utworzenie konta administratora
   - konfiguracja ścieżki dostępu do filmów
   - zalogowanie się na konto administratora
   - filmy są widoczne na stronie głównej po zalogowaniu
   - utworzenie kont dla domowników
     
   ![39_jellyfin_instalacja1](https://github.com/user-attachments/assets/a19b1a52-5b69-48a2-b282-bf19e92558ba)

   ![40_jellyfin_instalacja2](https://github.com/user-attachments/assets/08af1c61-b2d8-4416-87ae-177e4fdc9d19)
   
   ![41_jellyfin_instalacja3](https://github.com/user-attachments/assets/37c12f08-1b37-4839-8568-a06533bd9234)

   ![42_upload_filmów_na_serwer](https://github.com/user-attachments/assets/6642ec94-1272-4bf8-a12d-7c583ffb673e)

   ![43_filmy_na_serwerze](https://github.com/user-attachments/assets/2e903813-2438-424a-9a91-0d0a5624bb84)
   
   ![44_jellyfin_konfiguracja1](https://github.com/user-attachments/assets/d3d52e22-6160-47a6-af98-528810be316f)
   
   ![45_jellyfin_konfiguracja2](https://github.com/user-attachments/assets/0ecd9b23-4a35-4017-8a3b-b0f02b4a822c)

   ![46_jellyfin_logowanie](https://github.com/user-attachments/assets/2803b6a7-51da-498f-8d90-e91abb20248f)

   ![47_jellyfin_widoczne_filmy](https://github.com/user-attachments/assets/8b560c53-a64d-4c67-a43c-0a6d88c16596)

   ![48_jellyfin_nowy_user1](https://github.com/user-attachments/assets/6d02ae23-3baf-4310-ab9d-12f9c7ab0bb7)

   ![49_jellyfin_nowy_user2](https://github.com/user-attachments/assets/4a6e8634-55d1-4817-9dca-35537510a10c)

   ![50_jellyfin_userzy](https://github.com/user-attachments/assets/445c5404-97b4-49ff-af0c-c0c61c3a03dd)






   

   



   


   

   




   








   

















