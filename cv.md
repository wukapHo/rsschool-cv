Vyacheslav Likashkov's CV

My name is Vyacheslav Likashkov, beginner frontend developer. You can contaсt me via Telegram: @WukapHo

Now I'm studying on a course from the Rolling Scopes School. I have a broad knowledge of the design of computers. I have no work experience, but I have a great aspiration to learn it. So I hope I can become a good engineer.

My Skills

GitHub profile, up-to-date: wukapHo.
My Codewars profile: wukapHo.

Code Example

Cat and Mouse - 2D Version

function catMouse(map,moves){
    if (!map.includes('C') || !map.includes('m')) return 'boring without two animals';
    const arr = map.split('\n');
    let catY = 0;
    let catX = 0;
    let mouseY = 0;
    let mouseX = 0;
    for (i = 0; i < arr.length; i++) {
        let y = arr[i].indexOf('C');
        if (y !== -1) {
            catY = y;
            catX = i;
        }
        let Y = arr[i].indexOf('m');
        if (Y !== -1) {
            mouseY = Y;
            mouseX = i;
        }
    };
    if ((Math.abs(mouseY - catY) + Math.abs(mouseX - catX)) > moves) return 'Escaped!';
    return 'Caught!';
};

Friday the 13ths

function fridayTheThirteenths(start, end) {
    let current = new Date(start, 0, 13);
    let arr = [];
    if (arguments.length === 1) end = start;
    while (current.getFullYear() <= end) {
        let day = current.getDate();
        let weekDay = current.getDay();
        if (day === 13 && weekDay === 5) {
            arr.push(`${current.getMonth() + 1}/${day}/${current.getFullYear()}`);
        }
        current.setMonth(current.getMonth() + 1);
    }
    return arr.join(' ');
};

Education

MSUCE, Moscow State University of Civil Engineering, 2008...2012.

Languages

English, Basic level (A2).