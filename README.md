# InfoAktualne2023
           ViewBag.Liczba = zgloszenia.Where(x => x.Active).Count();
            ViewBag.Nieprzypisane = zgloszenia.Where(x => x.MechanikId == 1).Count();
            ViewBag.Zrealizowane = zgloszenia.Where(x => x.Active == false).Count();
