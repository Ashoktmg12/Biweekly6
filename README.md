using System;
using System.Collections.Generic;
using System.Linq;
using System.Threading.Tasks;
using Microsoft.AspNetCore.Mvc;

namespace Tutorial7Ex2._2.Controllers
{
    public class StudentController : Controller
    {
        public IActionResult Index()
        {
            return View();
        }
        public IActionResult Welcome(string name, int numTimes = 1)
        {
            ViewData["Message"] = "Hello it's ashok ";
            ViewData["NumTimes"] = numTimes;
            return View();
        }
        public IActionResult DescirbeMyself()
        {
           
            return View();
        }
    }
}
