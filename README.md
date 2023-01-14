
# InfoAktualne2023
        var zgloszenia = _context.Zgloszenias.Include(z => z.Magazyn).Include(z => z.Maszyna).Include(z => z.Mechanik).Include(z => z.User);
            ViewBag.Liczba = zgloszenia.Where(x => x.Active).Count();
            ViewBag.Nieprzypisane = zgloszenia.Where(x => x.MechanikId == 1).Count();
            ViewBag.Zrealizowane = zgloszenia.Where(x => x.Active == false).Count();
