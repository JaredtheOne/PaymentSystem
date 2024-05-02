-- phpMyAdmin SQL Dump
-- version 5.0.1
-- https://www.phpmyadmin.net/
--
-- Host: localhost:3307
-- Generation Time: Dec 08, 2021 at 04:35 PM
-- Server version: 10.4.11-MariaDB
-- PHP Version: 7.2.28

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
SET AUTOCOMMIT = 0;
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Database: `paymenttable`
--

-- --------------------------------------------------------

--
-- Table structure for table `paydetails`
--

CREATE TABLE `paydetails` (
  `id` int(11) NOT NULL,
  `name` text NOT NULL,
  `price` double NOT NULL,
  `balanceBefore` double NOT NULL,
  `balanceAfter` double NOT NULL,
  `itemName` text NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Dumping data for table `paydetails`
--

INSERT INTO `paydetails` (`id`, `name`, `price`, `balanceBefore`, `balanceAfter`, `itemName`) VALUES
(1, 'Jared', 120, 130, 10, 'ticket1'),
(2, 'Josh', 700, 750, 50, 'ticket 2'),
(3, 'Matt', 5000, 6000, 1000, 'ticket3');

--
-- Indexes for dumped tables
--

--
-- Indexes for table `paydetails`
--
ALTER TABLE `paydetails`
  ADD PRIMARY KEY (`id`);

--
-- AUTO_INCREMENT for dumped tables
--

--
-- AUTO_INCREMENT for table `paydetails`
--
ALTER TABLE `paydetails`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=4;
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
