## ⚛️ React Hooks Usage

This project uses **React Hooks** for state management and functional components.  

### Example: `useState`
```javascript
import React, { useState } from 'react';

function AttendanceCounter() {
  // useState hook to manage attendance count
  const [count, setCount] = useState(0);

  const markAttendance = () => {
    setCount(count + 1);
  };

  return (
    <div>
      <h2>Attendance Count: {count}</h2>
      <button onClick={markAttendance}>Mark Attendance</button>
    </div>
  );
}

export default AttendanceCounter;
