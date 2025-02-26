import 'package:flutter/material.dart';

void main() {
  runApp(RentalApp());
}

class RentalApp extends StatefulWidget {
  const RentalApp({super.key});

  @override
  State<RentalApp> createState() => _RentalAppState();
}

class _RentalAppState extends State<RentalApp> {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        body: SafeArea(
          child: ListView(
            children: [
              Padding(
                padding: EdgeInsets.only(
                  top: MediaQuery.of(context).size.height * 0.04,
                  left: MediaQuery.of(context).size.width * 0.04,
                  right: MediaQuery.of(context).size.width * 0.04,
                  bottom: MediaQuery.of(context).size.height * 0.03,
                ),
                child: Column(
                  crossAxisAlignment: CrossAxisAlignment.start,
                  children: [
                    // First container with search bar and tune icon
                    Container(
                      height: 215,
                      width: double.infinity,
                      color: const Color(0xFFECE6FB),
                      child: Padding(
                        padding: const EdgeInsets.only(top: 20, left: 18),
                        child: Column(
                          children: [
                            Text(
                              "Explore the World! By Travelling",
                              style: TextStyle(
                                fontSize: 30,
                                fontWeight: FontWeight.bold,
                              ),
                            ),
                            const SizedBox(height: 20),
                            Row(
                              children: [
                                // Search bar
                                Expanded(
                                  child: TextField(
                                    decoration: InputDecoration(
                                      filled: true,
                                      fillColor: Colors.white,
                                      border: OutlineInputBorder(
                                        borderRadius: BorderRadius.circular(15),
                                        borderSide: BorderSide.none,
                                      ),
                                      labelText: "Where did you go?",
                                      prefixIcon: const Icon(Icons.search),
                                    ),
                                  ),
                                ),
                                const SizedBox(width: 10),
                                // Tune icon
                                Padding(
                                  padding: const EdgeInsets.only(
                                      left: 25, right: 35),
                                  child: Container(
                                    height: 48,
                                    width: 48,
                                    decoration: BoxDecoration(
                                      color: Colors.white,
                                      borderRadius: BorderRadius.circular(15),
                                      boxShadow: [
                                        BoxShadow(
                                          color: Colors.grey,
                                          spreadRadius: 2,
                                          blurRadius: 5,
                                        ),
                                      ],
                                    ),
                                    child: IconButton(
                                      onPressed: () {},
                                      icon: const Icon(Icons.tune,
                                          color: Colors.black),
                                    ),
                                  ),
                                ),
                              ],
                            ),
                          ],
                        ),
                      ),
                    ),
                    const SizedBox(height: 20),

                    // Popular Locations Title
                    Padding(
                      padding: const EdgeInsets.only(left: 21),
                      child: Text(
                        "Popular Locations",
                        style: TextStyle(
                          fontSize: 28,
                          fontWeight: FontWeight.bold,
                        ),
                      ),
                    ),
                    const SizedBox(height: 23),

                    // Horizontal scrollable images for popular locations
                    SizedBox(
                      height: 180,
                      child: ListView(
                        scrollDirection: Axis.horizontal,
                        shrinkWrap: true,
                        physics: const BouncingScrollPhysics(),
                        children: [
                          // First image with left padding of 21
                          buildLocationImage(
                            'India',
                            'https://www.revv.co.in/blogs/wp-content/uploads/2019/11/self-drive-car-rental-delhi-gurgaon-noida_revv-blog.jpg',
                            leftPadding: 21,
                          ),
                          const SizedBox(width: 1),
                          buildLocationImage(
                            'Moscow',
                            'https://www.tripsavvy.com/thmb/F-m-fKVHCHPnER1vWEhpeL_prcU=/3588x2470/filters:fill(auto,1)/GettyImages-860736748-92a985df6f0c4854993acbb1f6ce0041.jpg',
                            leftPadding: 0,
                          ),
                          const SizedBox(width: 1),
                          buildLocationImage(
                            'USA',
                            'https://www.planetware.com/photos-large/USNY/usa-best-places-new-york.jpg',
                            leftPadding: 0,
                          ),
                          const SizedBox(width: 1),
                          buildLocationImage(
                            'Switzerland',
                            'https://c.myholidays.com/blog/blog/content/images/2021/04/Places-To-Visit-In-Switzerland.jpg',
                            leftPadding: 0,
                          ),
                          const SizedBox(width: 1),
                          buildLocationImage(
                            'Finland',
                            'https://www.visitfinland.com/dam/jcr:72b0d4b7-a3f9-439f-a555-c5ccc9b480d2/Finland_Porvoo_NikoLaurila6_.jpg',
                            leftPadding: 0,
                          ),
                        ],
                      ),
                    ),

                    const SizedBox(height: 17),

                    // Recommended Title
                    Padding(
                      padding: const EdgeInsets.only(left: 21),
                      child: Text(
                        "Recommended",
                        style: TextStyle(
                          fontSize: 28,
                          fontWeight: FontWeight.bold,
                        ),
                      ),
                    ),
                    const SizedBox(height: 23),

                    // Recommended locations with 4 more images
                    SizedBox(
                      height: 280,
                      child: ListView(
                        scrollDirection: Axis.horizontal,
                        shrinkWrap: true,
                        physics: const BouncingScrollPhysics(),
                        children: [
                          buildRecommendedLocation(
                            'https://www.travelplusstyle.com/wp-content/gallery/soneva-fushi_main-gallery/jungle-reserve-1_267_673.jpg',
                            '\$120',
                            'Corinthian Lake Breakfast included',
                            4.5,
                          ),
                          const SizedBox(width: 1),
                          buildRecommendedLocation(
                            'https://media.villagetaways.com/villas/maldives/160/20d2526b33cc53306b7fc81c6d18baaa_full.jpg',
                            '\$150',
                            'Maldives Beach Private pool',
                            4.7,
                          ),
                          const SizedBox(width: 1),
                          buildRecommendedLocation(
                            'https://www.maldivestourism.net/wp-content/gallery/constance-halaveli-resort-maldives/CHRMBPBeVilla12.jpg',
                            '\$200',
                            'Halalling Resort All-inclusive',
                            4.8,
                          ),
                          const SizedBox(width: 1),
                          buildRecommendedLocation(
                            'https://www.letsgomylove.com/wp-content/uploads/2022/09/hotel-waldegg-engelberg-suisse-11-1536x970.jpg',
                            '\$180',
                            'Swiss Alps Mountain view',
                            4.6,
                          ),
                          const SizedBox(width: 1),
                          buildRecommendedLocation(
                            'https://kalumatravel.co.uk/wp-content/uploads/2014/07/Hotel-Altapura-Exterior-II1.jpg',
                            '\$220',
                            'French Alps Ski-in, ski-out',
                            4.9,
                          ),
                        ],
                      ),
                    ),

                    const SizedBox(height: 25),

                    // Advertisement Section
                    Padding(
                      padding: const EdgeInsets.only(left: 20),
                      child: Container(
                        height: 300,
                        width: MediaQuery.of(context).size.width * 0.825,
                        decoration: BoxDecoration(
                          image: const DecorationImage(
                            image: NetworkImage(
                              'https://www.hollandamerica.com/blog/wp-content/uploads/2022/11/CelebratoinSale.jpg',
                            ),
                            fit: BoxFit.cover,
                          ),
                          borderRadius: BorderRadius.circular(15),
                        ),
                        child: Center(
                          child: Text(
                            '',
                            style: TextStyle(
                              fontSize: 24,
                              fontWeight: FontWeight.bold,
                              color: Colors.white,
                            ),
                          ),
                        ),
                      ),
                    ),

                    const SizedBox(height: 30),

                    // Most Viewed Section
                    Padding(
                      padding: const EdgeInsets.only(left: 21),
                      child: Text(
                        "Most Viewed",
                        style: TextStyle(
                          fontSize: 28,
                          fontWeight: FontWeight.bold,
                        ),
                      ),
                    ),
                    const SizedBox(height: 23),

                    // Vertical scrollable images for most viewed locations
                    SizedBox(
                      height: 900,
                      child: ListView(
                        scrollDirection: Axis.vertical,
                        shrinkWrap: true,
                        physics: const BouncingScrollPhysics(),
                        children: [
                          buildMostViewedLocation(
                            'https://www.travelplusstyle.com/wp-content/gallery/soneva-fushi_main-gallery/jungle-reserve-1_267_673.jpg',
                            '\$120',
                            'Corinthian Lake Breakfast included',
                            4.5,
                          ),
                          const SizedBox(height: 20),
                          buildMostViewedLocation(
                            'https://media.villagetaways.com/villas/maldives/160/20d2526b33cc53306b7fc81c6d18baaa_full.jpg',
                            '\$150',
                            'Maldives Beach Private pool',
                            4.7,
                          ),
                          const SizedBox(height: 20),
                          buildMostViewedLocation(
                            'https://www.maldivestourism.net/wp-content/gallery/constance-halaveli-resort-maldives/CHRMBPBeVilla12.jpg',
                            '\$200',
                            'Halalling Resort All-inclusive',
                            4.8,
                          ),
                        ],
                      ),
                    ),
                  ],
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }

  // Reusable method for location images (horizontal layout)
  Widget buildLocationImage(String location, String imageUrl,
      {double leftPadding = 0}) {
    return Padding(
      padding: EdgeInsets.only(
        left: leftPadding,
        right: 13,
      ),
      child: Stack(
        children: [
          ClipRRect(
            borderRadius: BorderRadius.circular(15),
            child: SizedBox(
              width: 130,
              height: 180,
              child: Image.network(
                imageUrl,
                fit: BoxFit.cover,
                loadingBuilder: (BuildContext context, Widget child,
                    ImageChunkEvent? loadingProgress) {
                  if (loadingProgress == null) {
                    return child;
                  } else {
                    return Center(
                      child: CircularProgressIndicator(
                        value: loadingProgress.expectedTotalBytes != null
                            ? loadingProgress.cumulativeBytesLoaded /
                                (loadingProgress.expectedTotalBytes ?? 1)
                            : null,
                      ),
                    );
                  }
                },
              ),
            ),
          ),
          Positioned(
            bottom: 20,
            left: 0,
            right: 0,
            child: Center(
              child: Text(
                location,
                style: const TextStyle(
                  color: Colors.white,
                  fontSize: 20,
                  fontWeight: FontWeight.bold,
                ),
              ),
            ),
          ),
        ],
      ),
    );
  }

  // Reusable method for recommended locations
  Widget buildRecommendedLocation(
      String imageUrl, String price, String location, double rating) {
    bool isHeartClicked = false;

    return StatefulBuilder(
      builder: (context, setState) {
        return Padding(
          padding: const EdgeInsets.only(left: 21, right: 13),
          child: Column(
            crossAxisAlignment: CrossAxisAlignment.start,
            children: [
              Stack(
                children: [
                  ClipRRect(
                    borderRadius: BorderRadius.circular(15),
                    child: SizedBox(
                      width: 280,
                      height: 180,
                      child: Image.network(
                        imageUrl,
                        fit: BoxFit.cover,
                      ),
                    ),
                  ),
                  // Heart Icon with Circle Border and White Background
                  Positioned(
                    top: 10,
                    right: 10,
                    child: Container(
                      decoration: BoxDecoration(
                        shape: BoxShape.circle,
                        color: Colors.white,
                        border: Border.all(
                          color: Colors.white,
                          width: 2,
                        ),
                      ),
                      child: IconButton(
                        onPressed: () {
                          setState(() {
                            isHeartClicked = !isHeartClicked;
                          });
                        },
                        icon: Icon(
                          Icons.favorite,
                          color: isHeartClicked ? Colors.red : Colors.grey,
                          size: 33,
                        ),
                      ),
                    ),
                  ),
                ],
              ),
              const SizedBox(height: 8),
              // Price and Star Rating in the same row
              Row(
                children: [
                  // Price with Bolt Icon
                  Row(
                    children: [
                      Text(
                        price,
                        style: const TextStyle(
                          fontSize: 18,
                          fontWeight: FontWeight.bold,
                        ),
                      ),
                      const Text(
                        '/ Night',
                        style: TextStyle(
                          fontSize: 18,
                          fontWeight: FontWeight.bold,
                        ),
                      ),
                      const SizedBox(width: 2),
                      const Icon(
                        Icons.bolt,
                        color: Colors.orange,
                        size: 18,
                      ),
                    ],
                  ),
                  // Star Rating
                  Padding(
                    padding: const EdgeInsets.only(left: 110),
                    child: Row(
                      children: [
                        const Icon(
                          Icons.star,
                          color: Colors.red,
                          size: 16,
                        ),
                        const SizedBox(width: 4),
                        Text(
                          rating.toString(),
                          style: const TextStyle(
                            fontSize: 14,
                            fontWeight: FontWeight.bold,
                            color: Colors.black,
                          ),
                        ),
                      ],
                    ),
                  ),
                ],
              ),
              const SizedBox(height: 4),
              // Location
              Text(
                location,
                style: const TextStyle(
                  fontSize: 16,
                  fontWeight: FontWeight.bold,
                  color: Colors.black,
                ),
              ),
              const SizedBox(
                height: 4,
              ),
              const Text(
                'Private room / 4 beds',
                style: TextStyle(
                  fontSize: 15,
                  color: Colors.black54,
                ),
              ),
            ],
          ),
        );
      },
    );
  }

  // Reusable method for most viewed locations
  Widget buildMostViewedLocation(
      String imageUrl, String price, String location, double rating) {
    bool isHeartClicked = false;

    return StatefulBuilder(
      builder: (context, setState) {
        return Padding(
          padding: const EdgeInsets.only(left: 21, right: 13),
          child: Column(
            crossAxisAlignment: CrossAxisAlignment.start,
            children: [
              Stack(
                children: [
                  ClipRRect(
                    borderRadius: BorderRadius.circular(15),
                    child: SizedBox(
                      width: MediaQuery.of(context).size.width * 0.9,
                      height: 180,
                      child: Image.network(
                        imageUrl,
                        fit: BoxFit.cover,
                      ),
                    ),
                  ),
                  // Heart Icon with Circle Border and White Background
                  Positioned(
                    top: 10,
                    right: 10,
                    child: Container(
                      decoration: BoxDecoration(
                        shape: BoxShape.circle,
                        color: Colors.white,
                        border: Border.all(
                          color: Colors.white,
                          width: 2,
                        ),
                      ),
                      child: IconButton(
                        onPressed: () {
                          setState(() {
                            isHeartClicked = !isHeartClicked;
                          });
                        },
                        icon: Icon(
                          Icons.favorite,
                          color: isHeartClicked ? Colors.red : Colors.grey,
                          size: 33,
                        ),
                      ),
                    ),
                  ),
                ],
              ),
              const SizedBox(height: 8),
              // Price and Star Rating in the same row
              Row(
                children: [
                  // Price with Bolt Icon
                  Row(
                    children: [
                      Text(
                        price,
                        style: const TextStyle(
                          fontSize: 18,
                          fontWeight: FontWeight.bold,
                        ),
                      ),
                      const Text(
                        '/ Night',
                        style: TextStyle(
                          fontSize: 18,
                          fontWeight: FontWeight.bold,
                        ),
                      ),
                      const SizedBox(width: 2),
                      const Icon(
                        Icons.bolt,
                        color: Colors.orange,
                        size: 18,
                      ),
                    ],
                  ),
                  // Star Rating
                  Padding(
                    padding: const EdgeInsets.only(left: 180),
                    child: Row(
                      children: [
                        const Icon(
                          Icons.star,
                          color: Colors.red,
                          size: 16,
                        ),
                        const SizedBox(width: 4),
                        Text(
                          rating.toString(),
                          style: const TextStyle(
                            fontSize: 14,
                            fontWeight: FontWeight.bold,
                            color: Colors.black,
                          ),
                        ),
                      ],
                    ),
                  ),
                ],
              ),
              const SizedBox(height: 4),
              // Location
              Text(
                location,
                style: const TextStyle(
                  fontSize: 16,
                  fontWeight: FontWeight.bold,
                  color: Colors.black,
                ),
              ),
              const SizedBox(
                height: 4,
              ),
              const Text(
                'Private room / 4 beds',
                style: TextStyle(
                  fontSize: 15,
                  color: Colors.black54,
                ),
              ),
            ],
          ),
        );
      },
    );
  }
}
