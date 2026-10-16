class TicketBooking {
    String passengerName;
    String bookingStatus;
    TicketBooking(String name) {
        passengerName = name;
        bookingStatus = "Confirmed";
    }
    void displayBooking() {
        System.out.println("Passenger Name: " + passengerName);
        System.out.println("Booking Status: " + bookingStatus);
        System.out.println("Thread Name: " +
                           Thread.currentThread().getName());
        System.out.println("----------------------");
    }
}
class BookingThread extends Thread {
    TicketBooking booking;
    BookingThread(String name) {
        booking = new TicketBooking(name);
    }
    public void run() {
        booking.displayBooking();
    }
}
class BookingRunnable implements Runnable {
    TicketBooking booking;
    BookingRunnable(String name) {
        booking = new TicketBooking(name);
    }
    public void run() {
        booking.displayBooking();
    }
}
public class Main {
    public static void main(String[] args) {
        BookingThread t1 = new BookingThread("Rahul");
        BookingThread t2 = new BookingThread("Priya");
        BookingRunnable r1 = new BookingRunnable("Amit");
        BookingRunnable r2 = new BookingRunnable("Sneha");
        Thread t3 = new Thread(r1, "Thread-3");
        Thread t4 = new Thread(r2, "Thread-4");
        t1.start();
        t2.start();
        t3.start();
        t4.start();
        try {
            t1.join();
            t2.join();
            t3.join();
            t4.join();
        } catch (InterruptedException e) {
            System.out.println("Thread interrupted.");
            Thread.currentThread().interrupt();
            return;
        }
        System.out.println(
            "All passenger booking requests processed successfully.");
    }
}
