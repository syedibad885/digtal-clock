function updateClock() {
    let now = new Date();
    let dname = now.getDay();
    let mo = now.getMonth();
    let dnum = now.getDate();
    let yr = now.getFullYear();
    let hou = now.getHours();
    let min = now.getMinutes();
    let sec = now.getSeconds();
    let per = "AM";
    if (hou == 0) {
      hou = 12;
    }
    if (hou > 12) {
      hou = hou - 12;
      per = "PM";
    }
    String.prototype.pad = function (digits) {
      let n = this.toString();
      while (n.length < digits) {
        n = "0" + n;
      }
      return n;
    };
    const months = [
      "January",
      "February",
      "March",
      "April",
      "May",
      "June",
      "July",
      "August",
      "September",
      "October",
      "November",
      "December",
    ];
    const daysOfWeek = [
      "Sunday",
      "Monday",
      "Tuesday",
      "Wednesday",
      "Thursday",
      "Friday",
      "Saturday",
    ];
    const ids = [
      "dayName",
      "month",
      "daynum",
      "year",
      "hour",
      "minutes",
      "seconds",
      "period",
    ];
    const values = [
      daysOfWeek[dname],
      months[mo],
      dnum.toString().pad(2),
      yr,
      hou.toString().pad(2),
      min.toString().pad(2),
      sec.toString().pad(2),
      per,
    ];
    for (let i = 0; i < ids.length; i++) {
      document.getElementById(ids[i]).textContent = values[i];
    }
  }
  
  function initClock() {
    updateClock();
    window.setInterval(updateClock, 1000);
  }
  initClock();