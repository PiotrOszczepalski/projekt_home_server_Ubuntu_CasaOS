Dokumentacja projektu

Home Server | DELL OptiPlex 5040 + Linux Ubuntu Server + CasaOS

Projekt domowego serwera w celu nauki administracji systemami Linux oraz zarządzania usługami sieciowymi. Utworzyłem środowisko serwerowe na bazie komputera DELL OptiPlex 5040, na którym zainstalowałem system Ubuntu Server oraz platformę CasaOS, umożliwiającą zarządzanie aplikacjami w środowisku webowym.

Cel projektu: serwis urządzenia (czyszczenie, wymiana pasty termoprzewodzącej), podpięcie dysków SSD oraz HDD, instalacja i administracja Ubuntu Server oraz CasaOS (SSH, partycjonowanie/montowanie dysków, zarządzanie usługami i aplikacjami kontenerowymi, monitorowanie wydajności), udostępnianie plików w sieci (SMB), wdrożenie usług Jellyfin (streaming multimediów) oraz Immich (lokalna chmura i backup zdjęć z urządzeń mobilnych), konfiguracja Pi-hole jako serwera DNS blokującego reklamy.

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

9) Jellyfin - możliwość oglądania filmów na urządzeniach mobilnych w sieci lokalnej:
   - instalacja Jellyfin na telefonie
   - połączenie się z domowym serwerem
   - zalogowanie się na konto domownika
   - filmy są dostępne
   - oglądanie jednego z filmów na telefonie

   ![51_jellyfin_telefon_instalacja](https://github.com/user-attachments/assets/f8fc6980-1a0f-46a8-a696-94f8f63c1d1c)

   ![52_jellyfin_połączenie_z_serwerem_na_telefonie](https://github.com/user-attachments/assets/2f5cc767-920b-416e-a303-52b9384d6098)
   
   ![53_jellyfin_logowanie_na_konto_domownika](https://github.com/user-attachments/assets/82e80203-8545-41f2-93e0-8ec85af9e358)

   ![54_jellyfin_na_telefonie](https://github.com/user-attachments/assets/7cfc508a-2e4f-4159-b79d-e1eabaf907c8)

   ![55_jellyfin_odtwarzanie_filmu_na_telefonie](https://github.com/user-attachments/assets/11e7ddbf-2c91-4c96-a50b-4f2656a6475e)

10) Jellyfin - możliwość oglądania różnych filmów na kilku urządzeniach w tym samym czasie (każdy domownik ma swoje własne konto):

    ![56_jellyfin_dwa_różne_urządzenia](https://github.com/user-attachments/assets/24d3730d-2152-4e55-8ba3-1c2aefbc420d)

11) Wdrożenie usługi Immich (domowa chmura i wygodny backup zdjęć z telefonu):
    - utworzenie dedykowanego punktu montowania, aby zdjęcia mogły zapisywać się na dysku HDD o pojemności 300 GB, a nie na dysku systemowym SSD o pojemności 120 GB (wcześniejsze automatyczne montowanie dysku HDD przez system nie zapewniało stabilności      wymaganej przez aplikacje kontenerowe)
    - zidentyfikowanie unikalnego identyfikatora partycji - UUID (blkid)
    - dodanie wpisu do pliku /etc/fstab (automatyczne montowanie dysku przy każdym starcie systemu)
    - przeładowanie konfiguracji oraz test poprawności montowania (systemctl daemon-reload, mount -a)
    - instalacja niestandardowa Immich (wskazanie dedykowanego dysku HDD)
    - utworzenie konta administratora
    - dostęp do panelu, Immich prawidłowo wykrywa dostępne miejsce - 292 GiB (HDD podłączony poprawnie)

    ![57_tworzenie_punktu_montowania_i_sprawdzenie_UUID](https://github.com/user-attachments/assets/bc720f27-2b62-44b4-a040-c73e1e5272e6)

    ![58_fstab](https://github.com/user-attachments/assets/dce512a5-77a2-4f0c-831e-68dabcc7c600)

    ![59_montowanie_dysku](https://github.com/user-attachments/assets/dd27f7ba-ebd7-484a-8b76-572ceac1ada0)

    ![60_immich_instalacja_custom](https://github.com/user-attachments/assets/f69712d3-7523-4ee6-8392-2011a6f18bd2)

    ![61_immich_lokalizacja_hdd](https://github.com/user-attachments/assets/f4689cc0-5556-4b99-868f-08bccc8352b1)

    ![62_immich_instalacja2](https://github.com/user-attachments/assets/b0f2f8b0-df78-44d0-8c5e-52d1c363904f)

    ![63_immich_instalacja3](https://github.com/user-attachments/assets/c32f5b8a-192e-4dae-a03a-e473f6e1128d)
    
    ![64_immich_konfiguracja](https://github.com/user-attachments/assets/8b8d2819-e431-4bfe-80ba-c56d2ba3cb06)

    ![65_immich_panel](https://github.com/user-attachments/assets/277155a9-7061-42a4-9d2a-f765b727648d)

12) Konfiguracja Immich na telefonie:
    - instalacja aplikacji
    - połączenie się z domowym serwerem
    - logowanie
    - upload zdjęć na serwer
    - zdjęcia są dostępne w aplikacji Immich na każdym urządzeniu w sieci lokalnej

    ![66_immich_instalacja_na_telefonie](https://github.com/user-attachments/assets/093909d6-2fe2-4e69-8088-907a6fc832dd)

    ![67_immich_konfiguracja_na_telefonie](https://github.com/user-attachments/assets/c371a04e-a58a-4953-ad38-841c4d2e0bab)

    ![68_immich_logowanie_na_telefonie](https://github.com/user-attachments/assets/777419f8-afbe-414b-8c50-df2bd2733b3f)

    ![69_immich_upload_zdjęć_z_galerii](https://github.com/user-attachments/assets/5531914c-c3c1-4ed3-8bc3-262d073df682)

    ![70_immich_upload_zdjęć_z_galerii2](https://github.com/user-attachments/assets/07f1f77e-6333-41b4-b40f-263095ea9b3f)

    ![71_immich_zdjęcia_na_serwerze](https://github.com/user-attachments/assets/9c252047-5265-4657-a6e4-734564aafd72)

13) Podłączenie tego samego dysku HDD do Jellyfin, aby również miał do niego dostęp (przykładowe odtworzenie muzyki zapisanej na HDD):

    ![72_jellyfin_dodanie_hdd](https://github.com/user-attachments/assets/df6ba485-484b-42cc-a2b7-0e44c328ab29)

    ![73_jellyfin_nowa_biblioteka](https://github.com/user-attachments/assets/b750eda9-b46f-4a2c-b326-61f1a1137270)

    ![74_jellyfin_nowa_biblioteka2](https://github.com/user-attachments/assets/bad79a4e-ba18-4e5b-8648-0c1d153fe201)

    ![75_jellyfin_muzyka_z_hdd](https://github.com/user-attachments/assets/167f052f-3fc9-4474-83a9-3c323530c53f)

14) Przygotowania do instalacji Pi-hole (serwera DNS blokującego reklamy w sieci lokalnej):
    - zajęty port 53 przez usługę systemową systemd-resolve, która domyślnie obsługuje lokalne rozwiązywanie nazw w systemie Ubuntu
    - wyłączenie mechanizmu DNSStubListener w pliku konfiguracyjnym /etc/systemd/resolved.conf
    - restart usługi
    - port 53 jest wolny i może być wykorzystany przez Pi-hole

    ![76_zajęty_port_53](https://github.com/user-attachments/assets/cf360e0e-1884-4dfa-873c-f0eecacec8c3)

    ![77_odblokowanie_portu_53](https://github.com/user-attachments/assets/e556bcfa-01b9-408b-9165-636c0e87c69b)

    ![78_restart_systemd-resolved](https://github.com/user-attachments/assets/2f082dff-b0f6-4254-97e4-37218324f266)

    ![79_wolny_port_53](https://github.com/user-attachments/assets/d881c05d-6706-4c15-b8fe-e8bb7a669a9d)

15) Instalacja Pi-hole:
    
    ![80_pi-hole_instalacja](https://github.com/user-attachments/assets/089c3f54-cbad-41c5-9bdc-1c310602e187)

    ![81_pi-hole_instalacja2](https://github.com/user-attachments/assets/1737847b-41b9-4d9a-aea9-bc814c713e36)

    ![82_pi-hole_instalacja3](https://github.com/user-attachments/assets/c946ecd3-1fb3-4ce5-ba8d-4156627072ae)

16) Konfiguracja Pi-hole:
    - zmiana domyślnego hasła
    - logowanie
    - dostęp do panelu
    - ustawienie domowego serwera jako główny adres DNS na routerze
    - wyłączenie DHCPv6, aby router nie przydzielał adresu DNS poprzez IPv6
    - poprawna konfiguracja, klienci w sieci otrzymują jako serwer DNS adres IP domowego serwera z zainstalowanym Pi-hole
    - blokowanie reklam na stronie Onetu (komputer stacjonarny)
    - blokowanie reklam na stronie Interii (smartfon)
    - blokowanie reklam w aplikacji (menedżer plików na telefonie)
    - lista zablokowanych reklam w panelu administracyjnym Pi-hole
    - lista klientów w sieci lokalnej korzystających z Pi-hole

    ![83_pi-hole_zmiana_domyślnego_hasła](https://github.com/user-attachments/assets/486f8f32-e29a-438f-80c3-1dfabd882b9c)

    ![84_pi-hole_logowanie](https://github.com/user-attachments/assets/b4e4933e-aeda-4cfa-8336-5502149547b5)

    ![85_pi-hole_panel](https://github.com/user-attachments/assets/5a7ce710-f7ca-4847-ac45-20e7aa83ebed)

    ![86_pi-hole_dns_na_routerze](https://github.com/user-attachments/assets/94950862-f190-4b3f-adf7-b9e788f326a5)

    ![87_pi-hole_wyłączenie_dhcp_ipv6_na_routerze](https://github.com/user-attachments/assets/19aab525-8c00-4b2d-bfbe-b6cf777ca0c0)

    ![88_pi-hole_dns_poprawna_konfiguracja_na_routerze](https://github.com/user-attachments/assets/b1b321e0-7e2d-4443-8aaf-05f69a29e21e)

    ![89_pi-hole_zablokowane_reklamy_na_stronie_onetu_na_komputerze](https://github.com/user-attachments/assets/157f39c6-88f2-4cb8-95be-9d90d3d2251c)

    ![90_pi-hole_zablokowane_reklamy_na_stronie_interii_na_telefonie](https://github.com/user-attachments/assets/726165fb-6d50-4ed5-a81f-cda7627e3dea)

    ![91_menedżer_plików_na_telefonie_przed_zastosowaniem_pi-hole_w_sieci](https://github.com/user-attachments/assets/02704849-99ff-4160-8db1-2b8dec29e6f7)

    ![92_menedżer_plików_na_telefonie_po_zastosowaniu_pi-hole_w_sieci](https://github.com/user-attachments/assets/8298cbe0-68c4-451b-8f3c-b64a62b8b9b8)

    ![93_pi-hole_lista_zablokowanych_reklam](https://github.com/user-attachments/assets/03c5a684-deab-4d11-836c-a059d9060304)

    ![94_pi-hole_lista_klientów](https://github.com/user-attachments/assets/69dd782c-e50d-4949-ac9b-1cc7c45e5cf2)

17) Monitorowanie wydajności serwera:
    - kondycja i temperatury dysków:
      - dysk SSD - zdrowy, temperatura 33 °C (bardzo dobra)
      - dysk HDD - zdrowy, temperatura 29 °C (również bardzo dobra, ale żeby ją sprawdzić trzeba użyć polecenia w terminalu smartctl -A /dev/sda2 | grep -i temperature - wynika to z ograniczeń CasaOS)
    - monitorowanie zużycia pamięci RAM (zużycie jest małe, 16 GB ram jest wystarczające do obsłużenia podstawowych aplikacji kontenerowych)
    - monitorowanie procesora (procesor i3 6100 pomimo posiadania 2 rdzeni daje sobie bez problemu radę przy podstawowych aplikacjach; dzięki wcześniejszej wymianie pasty termoprzewodzącej i wyczyszczeniu chłodzenia temperatura CPU jest bardzo niska -         ok. 25 °C)
    - monitorowanie stanu sieci:
      - 1 - stan bezczynności, minimalne transfery rzędu 1 KB/s
      - 2 - włączenie krótkiego filmiku w usłudze Jellyfin, zwiększenie skali do 5000 (aby zobrazować większy ruch), wzrost transferu i pik na wykresie (moment buforowania)




























    





   





   








   

   



   


   

   




   








   

















